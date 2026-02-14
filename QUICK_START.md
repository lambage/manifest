# Strike Force Hardware - Quick Reference Guide

## Quick Start Construction Guide

This is a condensed reference for building the Strike Force training device. For complete details, see [HARDWARE_DESIGN.md](HARDWARE_DESIGN.md).

## Recommended Build: Aluminum Frame

**Total Cost**: ~$1,200 | **Build Time**: 8-12 hours | **Skill Level**: Intermediate

### What You'll Need

#### Tools Required
- [ ] Drill with metal bits
- [ ] Saw (metal cutting - hacksaw or powered)
- [ ] Measuring tape and square
- [ ] Socket wrench set
- [ ] Allen key set
- [ ] Safety equipment (gloves, glasses)

#### Materials Checklist

**Frame** (~$600):
- [ ] (4) 2"x2"x1/4" aluminum square tube, 8ft
- [ ] (2) 2"x2"x1/4" aluminum square tube, 6ft  
- [ ] (4) 1.5"x1.5"x1/8" aluminum square tube, 4ft
- [ ] (2) 3"x3"x1/4" aluminum angle, 4ft

**Hardware** (~$150):
- [ ] (50) 1/4"-20 stainless bolts, washers, lock nuts
- [ ] (24) 3/8"-16 stainless bolts, washers, lock nuts
- [ ] (6) Quick-release pins
- [ ] (8) Steel corner brackets

**Targets** (~$300):
- [ ] (6) Foam pads, 2" thick (various sizes)
- [ ] (6) Plywood backing, 1/2"
- [ ] (6) Vinyl covers
- [ ] (6) Force sensors (FSR 402 or similar)

**Electronics** (~$150):
- [ ] ESP32 dev board
- [ ] LiPo battery 3.7V 5000mAh
- [ ] Weatherproof enclosure
- [ ] Wiring and connectors

**Base Weight** (~$100):
- [ ] (6) 50lb sandbags OR
- [ ] (12) 2" concrete pavers OR
- [ ] (1) 36"x36" steel plate

### Target Dimensions & Positions

| Target | Size | Height from Ground | Offset from Center |
|--------|------|-------------------|-------------------|
| Head | 10" x 12" | 66-70" | 0" |
| Chest | 10" x 12" | 48-52" | 0" |
| Right Arm | 8" x 10" | 48-52" | 14" right |
| Left Arm | 8" x 10" | 48-52" | 14" left |
| Right Kick | 12" x 14" | 24-30" | 12" right |
| Left Kick | 12" x 14" | 24-30" | 12" left |

*Heights adjustable for user size*

### Assembly Steps (2-3 hours)

1. **Build Base** (30 min)
   - Cut base frame to 48" x 48"
   - Add cross-bracing
   - Install ballast/weight

2. **Install Uprights** (30 min)
   - Attach vertical posts to base
   - Ensure vertical alignment
   - Add diagonal bracing

3. **Mount Target Arms** (45 min)
   - Install adjustable arms at each position
   - Add quick-release pins for height adjustment
   - Test adjustment mechanisms

4. **Prepare Targets** (60 min)
   - Mount sensors in foam pads
   - Attach plywood backing
   - Install vinyl covers
   - Wire sensors

5. **Install Electronics** (45 min)
   - Mount ESP32 in enclosure
   - Connect all sensors
   - Route cables through frame
   - Install battery

6. **Test & Adjust** (30 min)
   - Power on system
   - Test all sensors
   - Verify stability
   - Final adjustments

### Critical Safety Checks

- [ ] All bolts torqued properly
- [ ] Base weight minimum 250 lbs
- [ ] No sharp edges exposed
- [ ] Electrical connections sealed
- [ ] Frame doesn't wobble
- [ ] All sensors working

### Stability Test

**Before use, verify stability:**
1. Apply 100 lbs force to top target at 45° angle
2. Frame should not tip or move significantly
3. If unstable, add more base weight

## Budget Alternative: Wood/Metal Hybrid

**Total Cost**: ~$650 | **Build Time**: 6-8 hours | **Skill Level**: Beginner-Intermediate

### Key Differences
- Use 4x4" pressure-treated posts for uprights
- 2x6" lumber for base frame
- Steel reinforcement rods through posts
- Sandbags for weight
- Bolted construction (no welding)

### Advantages
- Lower cost
- Easier for DIY builders
- Common tools required
- Materials at any hardware store

### Disadvantages  
- Heavier (less portable)
- Less professional appearance
- May require more maintenance

## Troubleshooting

### Frame is unstable
- **Add more base weight** (target: 300+ lbs)
- Add diagonal bracing
- Widen base footprint
- Check all connections are tight

### Targets too stiff/soft
- Adjust foam thickness (2-3" range)
- Change foam density
- Add/remove backing material

### Sensors not detecting
- Check wiring connections
- Verify sensor positioning
- Test sensor with multimeter
- Update firmware calibration

### Height adjustment loose
- Replace quick-release pins
- Add lock nuts to bolts
- Check for worn holes
- Consider collar clamp system

## Maintenance Schedule

### Weekly
- Check all fasteners
- Inspect target pads
- Test sensors
- Clean surfaces

### Monthly
- Lubricate adjustments
- Check battery charge
- Inspect for damage
- Verify calibration

### Annual
- Full inspection
- Replace worn pads
- Refinish/repaint
- Update firmware

## Upgrade Paths

### Phase 1 (Basic)
- Fixed height targets
- Simple foam pads
- Basic sensors
- Manual operation

### Phase 2 (Intermediate)
- Adjustable heights
- Better padding/covers
- LED indicators
- App connectivity

### Phase 3 (Advanced)
- Gas-spring adjustment
- Professional padding
- Multiple sensor zones
- Advanced analytics

## Where to Buy Materials

### Metal & Hardware
- **McMaster-Carr**: mcmaster.com - Industrial supplies
- **Metal Supermarkets**: metalsupermarkets.com - Custom cutting
- **80/20 Inc**: 8020.net - Modular aluminum systems
- **Home Depot/Lowe's**: Hardware and fasteners

### Foam & Padding
- **Foam Factory**: foambymail.com - Custom foam cutting
- **American Foam**: americanfoam.com - High-density foam
- **Local upholstery shops**: Custom vinyl covers

### Electronics
- **Adafruit**: adafruit.com - ESP32, sensors
- **SparkFun**: sparkfun.com - Electronic components
- **Amazon**: ESP32 dev kits, batteries, enclosures

### Fabrication Services
- **Local metal fabricators**: Yellow pages/Google
- **TechShop/Maker Spaces**: Shared equipment access
- **Online services**: SendCutSend, eMachineShop

## Design Files Coming Soon

Future releases will include:
- [ ] 3D CAD models (FreeCAD, Fusion 360)
- [ ] 2D cut diagrams with dimensions
- [ ] Wiring diagrams for electronics
- [ ] 3D printable brackets and mounts
- [ ] Assembly videos/photos

## Support & Questions

- **Hardware Design**: See HARDWARE_DESIGN.md
- **Software Setup**: See strike_force_app/README.md
- **Firmware**: See strike_force_esp32/README.md
- **Issues**: Open issue on GitHub

## Safety Reminders

⚠️ Always wear appropriate safety equipment when constructing
⚠️ Verify structural integrity before use
⚠️ Keep workspace clean and organized
⚠️ Follow manufacturer guidelines for all tools
⚠️ When in doubt, consult a professional

---

**Ready to build?** Follow this guide along with HARDWARE_DESIGN.md for complete instructions!
