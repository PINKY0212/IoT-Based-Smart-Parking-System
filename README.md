# Smart Parking System

The **Smart Parking System** is an IoT-based solution designed to help drivers quickly locate vacant parking spaces. It automates entry/exit gates, tracks occupancy in real-time, and displays availability on an LCD screen and a mobile app. This system reduces parking time, minimizes congestion, and enhances user convenience through IoT automation.

## Key Features
- **Automated Gate Control**: IR sensor triggers servo motor to open/close the gate.  
- **Real-Time Occupancy Tracking**: Counter increments/decrements as vehicles enter/exit.  
- **Dynamic Display**: LCD screen shows available slots at the entrance.  
- **Mobile App Integration**: MQTT protocol updates parking status on a smartphone app.  
- **Capacity Management**: Blocks entry when parking is full.  

## Hardware Components
- **Raspberry Pi 3b+**: Central processing unit.  
- **IR Sensors**: Detect vehicle presence at gates and parking slots.  
- **Servo Motor**: Controls gate barrier (90° rotation).  
- **LCD Display**: Shows live parking availability.  

## Software & Technologies
- **Raspbian OS**: Operating system for Raspberry Pi.  
- **MQTT Protocol**: Enables app communication (publish-subscribe model).  
- **Custom Mobile App**: Built to display parking status remotely.

## How It Works
1. **Entry**:  
   - IR sensor detects a vehicle → Servo motor opens the gate.  
   - Counter increments; LCD and app update available slots.  
2. **Exit**:  
   - IR sensor triggers gate opening → Counter decrements.  
3. **Full Capacity**:  
   - System denies entry if slots are occupied.  

## Future Scope
- Integrate payment systems for reserved parking.  
- Add solar panels for energy-efficient operation.  
- Implement license plate recognition for security.
