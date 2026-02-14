# Strike Force Hardware Design Specification

## Overview
This document provides comprehensive hardware design specifications for the Strike Force martial arts training device. The system features 6 electronic targets that detect strikes from punches and kicks, integrated with ESP32 microcontroller and mobile app connectivity.

## Design Requirements

### Functional Requirements
- Support 6 strike targets positioned for realistic martial arts training
- Withstand repeated impacts from punches and kicks by adult users
- Maintain stability during vigorous training sessions
- Integrate ESP32 microcontroller and target sensors seamlessly
- Provide adjustable height positioning for different user sizes
- Allow easy access for maintenance and battery replacement

### Structural Requirements
- Support users up to 250 lbs (113 kg)
- Withstand strike forces up to 1000 lbs (4.4 kN)
- Maintain stability without tipping during use
- Weatherproof design for indoor/outdoor use (optional)
- Compact footprint (approximately 4ft x 4ft / 1.2m x 1.2m)
- Adjustable height range: 4ft to 6.5ft (1.2m to 2m)

## Target Placement Specifications

### Target Positions (for average height 5'10" / 178cm user)
1. **Head Target**: 66-70 inches (168-178cm) from ground
2. **Chest Target**: 48-52 inches (122-132cm) from ground  
3. **Right Arm Target**: 48-52 inches (122-132cm), 14 inches (36cm) right of center
4. **Left Arm Target**: 48-52 inches (122-132cm), 14 inches (36cm) left of center
5. **Right Torso/Kick Target**: 24-30 inches (61-76cm) from ground, 12 inches (30cm) right of center
6. **Left Torso/Kick Target**: 24-30 inches (61-76cm) from ground, 12 inches (30cm) left of center

## Recommended Construction Materials

### Option 1: Steel Frame Construction (Professional Grade)
**Pros**: Maximum durability, professional appearance, adjustable
**Cost**: $$$$

#### Materials:
- **Main Uprights**: 2" x 2" (50mm x 50mm) steel square tubing, 11 gauge wall thickness
- **Base Frame**: 2" x 2" steel square tubing with cross-bracing
- **Target Mounting Arms**: 1.5" x 1.5" steel square tubing with telescoping adjustment
- **Base Plate**: 1/4" (6mm) steel plate or weighted base
- **Surface Finish**: Powder-coated steel (black or custom color)
- **Fasteners**: Grade 8 bolts with lock washers

#### Base Weight Options:
1. **Steel Plate Base**: 4ft x 4ft x 1/4" steel plate (~400 lbs)
2. **Weighted Base Pockets**: Hollow base tubes filled with sand/concrete (~300 lbs)
3. **Bolt-Down**: Floor-mounted with expansion anchors

### Option 2: Aluminum Frame Construction (Semi-Professional)
**Pros**: Lighter weight, corrosion resistant, modern appearance
**Cost**: $$$

#### Materials:
- **Main Uprights**: 2" x 2" (50mm x 50mm) aluminum square tubing, 1/4" wall
- **Base Frame**: 2" x 2" aluminum square tubing with cross-bracing  
- **Target Mounting Arms**: 1.5" x 1.5" aluminum tubing with pin adjustment
- **Base Plate**: Aluminum with steel ballast pockets
- **Surface Finish**: Anodized aluminum or powder-coated
- **Fasteners**: Stainless steel bolts with nylon-insert lock nuts

#### Base Weight Options:
1. **Ballast Pockets**: Removable weight pockets (add 200-300 lbs)
2. **Wide Base Design**: 5ft x 4ft footprint for increased stability

### Option 3: Hybrid Wood/Metal Construction (Budget-Friendly)
**Pros**: Cost-effective, easier DIY construction, attractive appearance
**Cost**: $$

#### Materials:
- **Main Uprights**: 4x4" (100mm x 100mm) pressure-treated lumber with steel reinforcement
- **Base Frame**: 2x6" (50mm x 150mm) pressure-treated lumber
- **Target Mounting**: 2x4" lumber with steel brackets and piano hinges for adjustment
- **Base Weight**: Sandbags or concrete pavers (200-300 lbs)
- **Steel Reinforcement**: 1/2" threaded rod through uprights, steel corner brackets
- **Surface Finish**: Polyurethane or outdoor stain with protective coating

#### Construction Notes:
- Use lag bolts and construction adhesive for all joints
- Add diagonal bracing for lateral stability
- Encase electronics in waterproof boxes

### Option 4: Commercial Fitness Equipment Grade (Premium)
**Pros**: Professional appearance, gym-quality durability, best adjustability
**Cost**: $$$$$

#### Materials:
- **Frame**: 3" x 3" (75mm x 75mm) heavy-gauge steel tubing
- **Target Arms**: Gas-spring assisted adjustment with quick-release pins
- **Base**: Integrated weight stack or plate-loaded design
- **Surface**: Commercial grade powder coat with rubber bumpers
- **Padding**: High-density foam backing on targets

## Target Pad Specifications

### Impact Pad Requirements
- **Material**: High-density EVA foam or polyurethane padding
- **Thickness**: 2-3 inches (50-75mm)
- **Backing**: 1/2" (12mm) plywood or ABS plastic
- **Cover**: Vinyl or synthetic leather with reinforced stitching
- **Sensor Integration**: Cavity for force sensor and ESP32 components
- **Replacement**: Modular design for easy pad replacement

### Recommended Target Dimensions
- **Head/Chest Targets**: 10" x 12" (25cm x 30cm) 
- **Arm Targets**: 8" x 10" (20cm x 25cm)
- **Kick Targets**: 12" x 14" (30cm x 36cm)

## Structural Design Details

### Frame Design Recommendations

#### A-Frame Design (Recommended)
```
       [Head]
         |
    [LA] | [RA]
      \  |  /
       \ | /
        \|/
    ----===----  [Chest]
        /|\
       / | \
   [LK]  |  [RK]
         |
    =========== Base
```

**Advantages:**
- Excellent stability with wide base
- Natural ergonomics matching human striking patterns  
- Easy to adjust individual targets
- Self-supporting without wall mounting

#### Upright Post Design (Alternative)
```
    [Head]
      |
  [LA]|[RA]
      |
  [Chest]
      |
  [LK]|[RK]
      |
  ===Base===
```

**Advantages:**
- Compact footprint
- Simpler construction
- Easier to move/store
- Lower material cost

**Disadvantages:**
- Requires heavier base (400+ lbs)
- Less adjustment flexibility

### Base Design Options

#### Option A: Wide Platform Base
- Dimensions: 48" x 48" (122cm x 122cm)
- Weight: 300-400 lbs (136-181 kg)
- Materials: Steel plate or weighted frame
- Pros: Maximum stability, no floor mounting required
- Cons: Heavy, difficult to move

#### Option B: T-Base Design  
- Dimensions: 48" wide x 36" deep (122cm x 91cm)
- Weight: 200-300 lbs (91-136 kg)
- Materials: Steel or wood frame with ballast
- Pros: Good stability, easier to move
- Cons: Requires more floor space

#### Option C: Tripod Base
- Dimensions: 3 legs at 120° spacing, 30" radius (76cm)
- Weight: 150-250 lbs (68-113 kg)
- Materials: Steel or aluminum tubing
- Pros: Stable, efficient use of space
- Cons: More complex fabrication

## Height Adjustment Mechanisms

### Pin-and-Hole System (Simplest)
- Drill holes every 2 inches along uprights
- Use quick-release pins or bolts
- Pros: Simple, reliable, inexpensive
- Cons: Limited adjustment positions

### Telescoping with Collar Clamps
- Nested tube design with locking collars
- Infinite adjustment within range
- Pros: Precise positioning, easy to adjust
- Cons: May loosen with repeated impacts

### Gas-Spring Assisted (Premium)
- Hydraulic or pneumatic assistance
- Push-button release mechanism
- Pros: Easiest adjustment, professional feel
- Cons: Most expensive, requires maintenance

## Electronics Integration

### Weatherproofing
- House ESP32 and wiring in NEMA-rated enclosures (IP65 or better)
- Use waterproof cable glands for all wire pass-throughs
- Silicone seal all joints and mounting points
- Protect battery compartment from moisture

### Cable Management
- Run wires through hollow frame tubes when possible
- Use cable ties and clips for exposed runs
- Provide strain relief at all connection points
- Color-code or label all cables for maintenance

### Power Supply
- Rechargeable lithium battery pack (recommended)
- External DC power option with weatherproof connector
- Mount battery in accessible compartment with easy replacement
- Include LED indicators for battery status

## Assembly Instructions

### Recommended Assembly Steps

1. **Base Construction**
   - Assemble base frame with cross-bracing
   - Add ballast or weight before final assembly
   - Ensure level placement on floor

2. **Upright Installation**
   - Attach main uprights to base frame
   - Install diagonal bracing for lateral stability
   - Verify vertical alignment with level

3. **Target Arm Installation**
   - Mount adjustable target arms at appropriate heights
   - Install quick-release pins or adjustment mechanisms
   - Test adjustment range and locking

4. **Target Pad Mounting**
   - Install force sensors in target pad backing
   - Connect wiring to ESP32 controller
   - Mount pads to arms with secure fasteners
   - Verify sensor functionality

5. **Electronics Installation**
   - Mount ESP32 enclosure in protected location
   - Route and secure all cables
   - Install battery and test power
   - Perform calibration and testing

6. **Final Inspection**
   - Tighten all fasteners to specified torque
   - Test stability with applied force
   - Verify all sensors respond correctly
   - Apply final finish or protective coating

## Safety Considerations

### Structural Safety
- Regular inspection of all bolts and connections
- Check for cracks or damage to frame members
- Verify base weight is sufficient (should not tip with 45° force application)
- Ensure no sharp edges or pinch points
- Add rubber bumpers or edge protection

### Electrical Safety  
- Use properly rated components for all electronics
- Include fuse or circuit breaker protection
- Ground metal frames appropriately
- Keep all electrical connections dry and sealed
- Follow local electrical codes

### User Safety
- Provide adequate clearance around unit (minimum 6ft / 2m radius)
- Use on level, non-slip surface
- Post weight/height limits clearly
- Include emergency stop capability if powered
- Provide user manual with safety instructions

## Maintenance Requirements

### Regular Maintenance (Weekly)
- Check all fasteners for tightness
- Inspect target pads for wear or damage
- Test all sensors and confirm operation
- Clean surfaces and remove debris

### Periodic Maintenance (Monthly)
- Lubricate adjustment mechanisms
- Check battery charge and connections
- Inspect frame for corrosion or damage
- Verify calibration of force sensors

### Annual Maintenance
- Complete disassembly and inspection
- Replace worn target pads
- Repaint or refinish as needed
- Update firmware if available

## Cost Estimates (USD)

### Budget Build (Option 3 - Hybrid Wood/Metal)
- Materials: $200-400
- Hardware: $50-100
- Target Pads: $150-250
- Electronics: $100-150 (ESP32 + sensors)
- **Total: $500-900**

### Mid-Range Build (Option 2 - Aluminum Frame)
- Materials: $500-800
- Hardware: $100-150
- Target Pads: $200-350
- Electronics: $100-150
- **Total: $900-1,450**

### Professional Build (Option 1 - Steel Frame)
- Materials: $800-1,200
- Fabrication: $500-1,000 (if welded)
- Hardware: $150-250
- Target Pads: $300-500
- Electronics: $150-200
- **Total: $1,900-3,150**

### Premium Build (Option 4 - Commercial Grade)
- Materials: $1,500-2,500
- Fabrication: $1,000-2,000
- Hardware: $300-500
- Target Pads: $500-800
- Electronics: $200-300
- **Total: $3,500-6,100**

## Recommended Build for Most Users

### **Option 2: Aluminum Frame Construction**

This option provides the best balance of:
- **Durability**: Strong enough for vigorous training
- **Weight**: Light enough to move when needed (~150 lbs assembled)
- **Appearance**: Modern, professional look
- **Cost**: Reasonable for quality delivered (~$1,200 total)
- **Adjustability**: Easy height modifications
- **Maintenance**: Low maintenance, corrosion-resistant

### Detailed Parts List (Aluminum Build)

#### Frame Materials
- (4) 2" x 2" x 1/4" aluminum square tubing, 8ft lengths
- (2) 2" x 2" x 1/4" aluminum square tubing, 6ft lengths  
- (4) 1.5" x 1.5" x 1/8" aluminum square tubing, 4ft lengths
- (2) 3" x 3" x 1/4" aluminum angle iron, 4ft lengths (base)

#### Hardware
- (50) 1/4"-20 x 1" stainless steel bolts with nylon-insert lock nuts
- (24) 3/8"-16 x 2" stainless steel bolts with washers and lock nuts
- (6) Quick-release pins with detent balls
- (8) Steel corner gussets, 3" x 3"
- (100) Stainless steel washers, various sizes

#### Target Pads & Sensors
- (6) High-density foam pads (custom cut: 2" thick)
- (6) 1/2" plywood backing boards (cut to target sizes)
- (6) Vinyl covers with reinforced edges
- (6) Force sensors (FSR 402 or similar)
- (6) Sensor mounting brackets

#### Electronics
- (1) ESP32 development board with WiFi/Bluetooth
- (1) Custom PCB or breadboard for connections
- (1) LiPo battery pack, 3.7V 5000mAh
- (1) Battery management system (BMS)
- (6) Signal conditioning circuits for sensors
- (20ft) Shielded cable for sensor wiring
- (1) Waterproof enclosure for ESP32 (NEMA 4X rated)

#### Base Ballast
- (6) Sandbags, 50 lbs each OR
- (12) Concrete pavers, 2" thick OR  
- (1) Steel plate, 36" x 36" x 1/4"

#### Finishing
- (1qt) Metal primer
- (1qt) Powder coat or enamel paint
- (1) Package rubber edge guards
- (4) Rubber feet or floor protectors

## CAD Files and Templates

*(Note: CAD files would be added in future versions)*

Consider using these free CAD tools for design:
- **FreeCAD**: Open-source parametric 3D modeler
- **Fusion 360**: Free for hobbyists, excellent for mechanical design
- **SketchUp**: Easy to use for basic structural design
- **Tinkercad**: Browser-based, good for beginners

## Fabrication Options

### DIY Construction
- All designs can be built with basic tools (saw, drill, wrench)
- Option 3 (wood/metal hybrid) is easiest for beginners
- Options 1-2 require metal cutting/drilling tools
- No welding required if using bolted construction

### Professional Fabrication
- Local metal fabricators can cut and drill per specifications
- Welding services available for permanent construction
- Powder coating services for professional finish
- Average fabrication cost: $500-1,500 depending on complexity

### Recommended Fabricators/Suppliers
- **Metal Supermarkets**: Custom metal cutting and materials
- **McMaster-Carr**: Hardware, fasteners, and industrial supplies
- **80/20 Inc**: Modular aluminum framing systems (easy assembly)
- **Local welding shops**: Custom fabrication services

## Design Improvements Over Current Prototype

### Current Issues Addressed:
1. **Aesthetics**: Professional powder-coated finish vs. raw materials
2. **Stability**: Engineered base design vs. cement bucket
3. **Adjustability**: Multiple height positions vs. fixed posts
4. **Durability**: Engineered connections vs. ad-hoc construction
5. **Portability**: Designed weight distribution vs. overly heavy
6. **Safety**: Smooth surfaces and proper engineering vs. rough prototype
7. **Maintenance**: Modular replaceable components vs. permanent construction

## Next Steps

1. **Select Design Option**: Choose from Options 1-4 based on budget and skill
2. **Create Detailed Plans**: Develop cut list and assembly drawings
3. **Source Materials**: Order or purchase materials from suppliers
4. **Fabricate Components**: Cut, drill, and prepare all parts
5. **Assemble Frame**: Follow assembly instructions step-by-step
6. **Install Electronics**: Integrate ESP32 and sensors
7. **Test and Calibrate**: Verify operation and adjust as needed
8. **Finish and Protect**: Apply final coating and protective elements

## Additional Resources

### Recommended Reading
- "Welding For Dummies" - if pursuing welded construction
- "The Art and Science of Martial Arts Training Equipment"
- Metal framing guides from manufacturers
- ESP32 integration tutorials

### Online Communities
- r/metalworking - Reddit community for fabrication advice
- r/DIY - General construction help
- Martial arts equipment forums
- Maker spaces and local workshops

## Revision History
- v1.0 (2026-02-14): Initial hardware design specification

## Contact & Support
For questions about this design or implementation assistance, please open an issue in the GitHub repository.
