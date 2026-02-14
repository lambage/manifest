# Strike Force - Safety & Testing Guidelines

## Safety Overview

The Strike Force training device is designed for vigorous martial arts training with significant impact forces. Proper construction, testing, and maintenance are critical for user safety.

---

## PRE-USE SAFETY CHECKLIST

### Before Every Training Session

- [ ] **Visual Inspection**: Check frame for cracks, bends, or damage
- [ ] **Fastener Check**: Verify all bolts are tight (hand-check, no rattling)
- [ ] **Base Stability**: Ensure base weight is secure and hasn't shifted
- [ ] **Target Pads**: Inspect for tears, loose covers, or exposed sensors
- [ ] **Electronics**: Verify power indicator LED is on, sensors respond
- [ ] **Clearance**: Confirm 6-foot radius is clear of obstacles
- [ ] **Floor Surface**: Check for level, non-slip surface

### Weekly Maintenance Checks

- [ ] **Torque Check**: Use torque wrench on critical bolts
- [ ] **Adjustment Pins**: Verify quick-release pins engage fully
- [ ] **Wiring**: Inspect for fraying, exposed wires, or loose connections
- [ ] **Battery**: Check charge level and connections
- [ ] **Padding**: Compress foam to check for permanent deformation
- [ ] **Clean**: Wipe down all surfaces, remove debris

### Monthly Maintenance

- [ ] **Full Disassembly Check**: Remove targets, inspect mounting points
- [ ] **Lubrication**: Apply dry lubricant to sliding adjustment mechanisms
- [ ] **Electronics Test**: Test all sensors individually, verify readings
- [ ] **Calibration**: Recalibrate force sensors if needed
- [ ] **Documentation**: Record any issues or repairs in maintenance log

---

## STRUCTURAL TESTING REQUIREMENTS

### Initial Assembly Testing

#### Test 1: Static Load Test
**Purpose**: Verify structural integrity under load  
**Procedure**:
1. With unit assembled and weighted, apply 150 lbs static load to head target
2. Hold for 30 seconds
3. Check for deflection greater than 1 inch
4. Inspect all joints for movement or cracking

**Pass Criteria**: Less than 1" deflection, no visible damage

#### Test 2: Lateral Stability Test  
**Purpose**: Ensure unit won't tip during side strikes  
**Procedure**:
1. Apply 100 lbs force at 45° angle to highest target
2. Apply force from multiple directions (N, S, E, W)
3. Measure base movement

**Pass Criteria**: Base lifts less than 1" on any side, no tipping

#### Test 3: Impact Test
**Purpose**: Verify unit withstands repeated strikes  
**Procedure**:
1. Strike each target 20 times with moderate force
2. Strike each target 5 times with maximum safe force
3. Inspect frame, targets, and sensors after test

**Pass Criteria**: No damage to structure, all sensors still functional

#### Test 4: Vibration Test
**Purpose**: Ensure fasteners remain tight under use  
**Procedure**:
1. Perform 50 strikes across all targets over 5 minutes
2. Immediately check all fasteners for loosening
3. Re-tighten any loose fasteners

**Pass Criteria**: No more than 2 fasteners require tightening

---

## ELECTRICAL SAFETY

### Safe Electronics Installation

1. **Insulation**: All electrical connections must be insulated
2. **Waterproofing**: All outdoor/exposed electronics in NEMA-rated enclosures
3. **Strain Relief**: Cable entry points must have proper strain relief
4. **Fusing**: Include 5A fuse or circuit breaker in battery circuit
5. **Voltage**: Verify voltage levels with multimeter before connecting ESP32
6. **Polarity**: Double-check battery polarity before connecting

### Electrical Testing Procedure

#### Test 1: Continuity Check
- [ ] Verify no shorts between power and ground
- [ ] Check all sensor connections for continuity
- [ ] Verify proper ground connections on metal frame

#### Test 2: Voltage Test
- [ ] Battery voltage: 3.7-4.2V (LiPo)
- [ ] ESP32 input: 3.3V or 5V as specified
- [ ] Sensor bias voltage: Per sensor datasheet

#### Test 3: Sensor Response Test
- [ ] Each sensor should output 0V at rest
- [ ] Each sensor should output increasing voltage with pressure
- [ ] All sensors should respond independently

#### Test 4: Communication Test
- [ ] ESP32 connects to WiFi/Bluetooth successfully
- [ ] Mobile app receives sensor data
- [ ] No data dropouts during 5-minute test

### Electrical Safety Rules

⚠️ **NEVER**:
- Work on electronics while powered
- Use damaged cables or connectors
- Bypass fuses or protection circuits
- Expose electronics to water without proper sealing
- Exceed voltage/current ratings of components

✅ **ALWAYS**:
- Disconnect battery before working on circuits
- Use properly rated wire gauges
- Include overcurrent protection
- Keep connectors clean and dry
- Follow manufacturer datasheets

---

## USER SAFETY GUIDELINES

### Before Training

1. **Warm Up**: Always warm up muscles before striking
2. **Inspect**: Perform pre-use safety checklist
3. **Clear Area**: Ensure 6-foot clearance around unit
4. **Proper Form**: Use correct martial arts striking technique
5. **Protective Gear**: Wear hand wraps or gloves for hand strikes

### During Training

1. **Start Light**: Begin with light strikes, gradually increase intensity
2. **Listen to Your Body**: Stop if you feel pain in joints or muscles
3. **Proper Technique**: Focus on form, not just force
4. **Rest Between Sets**: Allow adequate recovery time
5. **Stay Alert**: Watch for equipment shifting or unusual sounds

### After Training

1. **Cool Down**: Perform cool-down stretches
2. **Ice If Needed**: Ice any sore joints or bruises
3. **Inspect Equipment**: Check for any damage from session
4. **Report Issues**: Document any equipment problems
5. **Secure Unit**: Ensure unit is stable and secured

### Contraindications

**Do NOT use this equipment if you have**:
- Recent hand, wrist, elbow, shoulder, knee, or ankle injuries
- Osteoporosis or brittle bones
- Heart conditions without doctor approval
- High blood pressure without doctor approval
- Are pregnant without doctor approval
- Under 12 years old without adult supervision

---

## INSTALLATION SAFETY

### Location Requirements

#### Indoor Installation
- [ ] Minimum 8-foot ceiling height
- [ ] 6-foot clearance radius around unit
- [ ] Level floor (within 1° of horizontal)
- [ ] Floor load capacity: 100 lbs per square foot minimum
- [ ] Good ventilation (if batteries charging)
- [ ] Away from water sources

#### Outdoor Installation (Optional)
- [ ] Covered area (patio, pavilion) or weatherproof design
- [ ] Solid, level base (concrete pad recommended)
- [ ] Protected from direct sun exposure (electronics)
- [ ] Drainage to prevent water pooling
- [ ] Secured against high winds if semi-permanent

### Environmental Conditions

**Operating Conditions**:
- Temperature: 32°F to 95°F (0°C to 35°C)
- Humidity: 10% to 80% non-condensing
- Altitude: Sea level to 6,000 feet

**Storage Conditions**:
- Temperature: 0°F to 110°F (-18°C to 43°C)
- Dry location, protected from moisture
- Batteries removed or disconnected for long-term storage

---

## IMPACT FORCE GUIDELINES

### Recommended Force Levels

| User Experience | Max Impact Force | Target PSI |
|----------------|------------------|------------|
| Beginner (learning form) | 50-100 lbs | Low |
| Intermediate (building power) | 100-300 lbs | Medium |
| Advanced (full power) | 300-600 lbs | High |
| Professional (competition level) | 600-1000 lbs | Very High |

**Note**: Unit is designed for up to 1000 lbs peak impact, but sustained use at maximum force will reduce equipment life.

### Force Progression

**Week 1-2**: Maximum 25% intensity, focus on form  
**Week 3-4**: Maximum 50% intensity, build technique  
**Week 5-8**: Maximum 75% intensity, increase power  
**Week 9+**: Full intensity as comfortable

---

## EMERGENCY PROCEDURES

### Equipment Failure During Use

**If unit begins to tip**:
1. Step back immediately
2. Allow unit to settle or fall (do not try to catch)
3. Ensure no one is in falling path
4. Once stable, power off electronics
5. Inspect for damage before re-use

**If target detaches**:
1. Stop training immediately
2. Power off unit
3. Inspect mounting hardware
4. Do not use until repaired and tested

**If electrical sparking/smoking**:
1. Do not touch metal frame
2. Disconnect battery immediately if safe to do so
3. Move away from unit
4. Use fire extinguisher if needed (Class C for electrical)
5. Do not use until inspected and repaired by qualified person

### Injury Response

**For minor bruises/sprains**:
1. Stop training immediately
2. Apply RICE protocol (Rest, Ice, Compression, Elevation)
3. Monitor for 24 hours
4. Seek medical attention if worsening

**For suspected fracture or severe injury**:
1. Stop training immediately
2. Do not move injured area
3. Call emergency services (911 in US)
4. Apply ice while waiting for help
5. Document incident for equipment review

---

## LOAD TESTING PROTOCOL (Detailed)

### Required Equipment
- Bathroom scale or hanging scale (0-300 lbs)
- Level
- Measuring tape
- Assistant for safety
- Camera for documentation

### Test Procedure

#### Setup (10 minutes)
1. Place unit on level surface
2. Ensure all assembly is complete per instructions
3. Verify base weight is installed (minimum 250 lbs)
4. Have assistant standing by for safety

#### Static Tests (20 minutes)

**Test A: Vertical Load - Head Target**
1. Position scale on floor, place board on scale
2. Press down on head target onto board/scale
3. Record force at which unit becomes unstable (tipping point)
4. **Target**: Tipping point > 150 lbs

**Test B: Vertical Load - Each Target**
1. Repeat Test A for all 6 targets
2. Record results for each
3. **Target**: All targets > 100 lbs tipping point

**Test C: Lateral Load**
1. Apply force parallel to ground on head target
2. Measure distance base slides or lifts
3. Record force at which movement occurs
4. **Target**: Movement > 75 lbs force

#### Dynamic Tests (30 minutes)

**Test D: Repeated Strike Test**
1. Strike head target 20 times at 50% intensity
2. Inspect frame and fasteners
3. Strike chest target 20 times at 50% intensity
4. Inspect frame and fasteners
5. Continue for all targets
6. **Target**: No visible loosening or damage

**Test E: Maximum Force Test**
1. Strike each target once at 75% intensity
2. Inspect after each strike
3. If no issues, strike once at 90% intensity
4. **Target**: No damage at 90% intensity

**Test F: Endurance Test**
1. Perform 100 strikes distributed across all targets
2. Varying intensity (50-75%)
3. Inspect every 25 strikes
4. **Target**: No damage or loosening after 100 strikes

### Documentation

Record all test results in maintenance log:
- Date and time of testing
- Tester name(s)
- Measurements and observations
- Pass/fail for each test
- Photos of any damage or issues
- Repairs or adjustments made

### Retest Requirements

**Retest immediately if**:
- Any test failure
- After any repairs to frame
- After replacing major components
- After incident or damage

**Retest periodically**:
- Every 6 months for regular use
- Every 3 months for heavy use (daily)
- Annually for light use (weekly)

---

## SENSOR CALIBRATION

### When to Calibrate

- After initial assembly
- After replacing any sensor
- If readings seem inaccurate
- Every 6 months for accuracy

### Calibration Procedure

1. **Zero Calibration**:
   - Remove all load from targets
   - Record baseline reading from each sensor
   - Adjust software to set baseline to zero

2. **Span Calibration**:
   - Apply known weight (e.g., 50 lbs using scale method)
   - Record sensor output
   - Adjust software calibration factor
   - Verify reading matches applied weight

3. **Linearity Check**:
   - Apply 25 lbs, 50 lbs, 75 lbs, 100 lbs sequentially
   - Verify readings are proportional
   - Note any non-linearity for software compensation

4. **Repeatability Test**:
   - Apply and remove 50 lbs force 10 times
   - Record readings each time
   - Verify standard deviation < 5%

### Calibration Documentation

Maintain calibration log with:
- Date of calibration
- Sensor ID/location
- Calibration values/factors
- Test results
- Technician signature

---

## QUALITY CONTROL CHECKLIST

### Final Assembly QC (Before First Use)

#### Structural
- [ ] All cuts are square and smooth
- [ ] All holes are drilled properly and deburred
- [ ] Frame is properly aligned (vertical within 1°)
- [ ] All bolts torqued to specification
- [ ] Welds (if applicable) are complete and sound
- [ ] No sharp edges or protrusions
- [ ] Powder coat/paint is complete and smooth
- [ ] Base weight is secured and won't shift

#### Targets
- [ ] Foam is properly sized and centered
- [ ] Vinyl covers are tight and properly sewn
- [ ] Sensors are centered in targets
- [ ] All wiring is secured and not pinched
- [ ] Target arms adjust smoothly
- [ ] Quick-release pins engage fully
- [ ] Targets are at correct heights for user

#### Electrical
- [ ] All connections are soldered or crimped properly
- [ ] All connections are insulated
- [ ] Wiring is routed safely (no pinch points)
- [ ] Enclosures are sealed against moisture
- [ ] Battery is charged and connections secure
- [ ] ESP32 powers on and connects to app
- [ ] All sensors respond to pressure
- [ ] No shorts or incorrect voltages

#### Safety
- [ ] All pre-use checklist items verified
- [ ] Load testing completed and passed
- [ ] User manual and safety instructions provided
- [ ] Warning labels affixed
- [ ] Emergency contact information posted
- [ ] Maintenance log started

---

## WARRANTY & LIABILITY

### Recommended User Agreement

Users of this equipment should acknowledge:
1. This is a DIY project with inherent risks
2. Proper assembly is critical for safety
3. Regular inspection and maintenance is required
4. User assumes all risk of injury
5. Equipment is used at own risk
6. Consult doctor before beginning training program

### Liability Waiver Template

Consider having users sign a waiver:
- Acknowledgment of risks
- Agreement to follow safety guidelines
- Release from liability for injury
- Confirmation of proper assembly/maintenance
- Emergency contact information

**Consult a lawyer** for proper waiver language in your jurisdiction.

---

## TROUBLESHOOTING SAFETY ISSUES

### Issue: Unit feels unstable during use

**Potential Causes**:
- Insufficient base weight
- Uneven floor surface
- Loose fasteners
- Improper assembly

**Solutions**:
1. Add more base weight (target 350+ lbs)
2. Shim base to level on floor
3. Tighten all fasteners
4. Verify assembly per instructions
5. Add wider base footprint

### Issue: Target arms are loose or wobble

**Potential Causes**:
- Worn quick-release pin holes
- Insufficient clamping force
- Damaged adjustment mechanism

**Solutions**:
1. Replace quick-release pins
2. Add lock collars or set screws
3. Drill new holes if existing are worn
4. Replace damaged components
5. Consider welding for permanent height

### Issue: Sensors give erratic readings

**Potential Causes**:
- Loose wiring connections
- Damaged sensor
- Moisture in connections
- EMI from nearby equipment

**Solutions**:
1. Check and reseat all connections
2. Test sensor with multimeter
3. Seal any moisture entry points
4. Use shielded cable
5. Replace damaged sensors
6. Recalibrate sensors

### Issue: Padding is wearing quickly

**Potential Causes**:
- Insufficient foam density
- Improper strike technique
- Excessive force for padding type

**Solutions**:
1. Use higher density foam (HD-36 or better)
2. Add thicker padding (3" instead of 2")
3. Review striking technique
4. Add protective vinyl cover
5. Rotate targets to distribute wear

---

## DISPOSAL & DECOMMISSIONING

### Safe Disassembly

When permanently retiring equipment:
1. Disconnect and remove battery
2. Remove all electronics
3. Disassemble targets
4. Unbolt frame components
5. Separate materials for recycling

### Recycling Guidelines

- **Aluminum/Steel**: Recycle at metal scrap yard
- **Electronics**: E-waste recycling facility
- **Batteries**: Battery recycling (never trash)
- **Foam**: Check for foam recycling programs
- **Vinyl**: May be recyclable as #4 plastic
- **Wood**: Recycle or repurpose

### Donation Considerations

If donating used equipment:
1. Perform complete safety inspection
2. Replace any worn components
3. Provide all documentation
4. Demonstrate proper use
5. Transfer maintenance log
6. Include liability waiver for new user

---

## ADDITIONAL RESOURCES

### Safety Standards References
- ASTM F1749: Standard Specification for Fitness Equipment
- CPSC Guidelines: Consumer Product Safety Commission
- OSHA: Occupational Safety Guidelines (if commercial use)

### First Aid Resources
- Red Cross First Aid Guide
- Sports Injury First Aid
- Local emergency services: 911 (US)

### Equipment Inspection Services
- Local structural engineers
- Certified welding inspectors
- Electrical safety inspectors

---

## REVISION HISTORY

- v1.0 (2026-02-14): Initial safety and testing guidelines

---

## CONTACT FOR SAFETY CONCERNS

For questions about safety or to report safety issues:
- Open issue on GitHub repository
- Include photos and detailed description
- Note any injuries or near-misses
- Suggest improvements to safety guidelines

**Remember**: Safety is everyone's responsibility. If something doesn't seem right, stop and investigate before continuing.

⚠️ **When in doubt, err on the side of caution!** ⚠️
