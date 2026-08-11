# The Crux

A keyboard with

- An [nRF52840](https://www.nordicsemi.com/Products/nRF52840) System on Chip ([datasheet](https://docs.nordicsemi.com/bundle/ps_nrf52840/page/keyfeatures_html5.html))
  - Programmer
- [DRV5056](https://www.ti.com/product/DRV5056) Linear Hall-Effect Sensors ([datasheet](https://www.ti.com/lit/ds/symlink/drv5056.pdf))
  - Will it work reversed?
- [TS5A3359](https://www.ti.com/product/TS5A3359) Analog Multiplexers ([datasheet](https://www.ti.com/lit/ds/symlink/ts5a3359.pdf))
- [SK6812MINI-E](https://www.adafruit.com/product/4960) Addressable LEDs ([datasheet](https://cdn-shop.adafruit.com/product-files/4960/4960_SK6812MINI-E_REV02_EN.pdf), [buy](https://www.adafruit.com/product/4960))
- [GATERON Full POM Low Profile Magnetic Jade Pro Switches](https://www.gateron.com/products/gateron-full-pom-low-profile-magnetic-jade-pro-switch-set?VariantsId=10870) ([datasheet](https://www.gateron.com/u_file/2506/10/file/GATERONLowProfileMagneticJadeProSwitchSPEC-KS-33D-001KS-33DD10B060NW-D276KS-33D.pdf), [buy](https://www.maxgaming.com/en/switches/jade-pro-full-pom-low-profile-switch))
- Power switch
- Battery, charging (also when powered off)
- the works as a plate part

## Power

- Sources (protect if they are wrong)
  - USB (5V)
  - Battery (2.5-4.5V)

---

- USB connected, jack connected
- USB connected, jack disconnected
- USB disconnected, jack connected
- USB disconnected, jack disconnected

## Power TODO

- do i even want a power switch?
- power can come from other side
- thingy to not burn when taking jack out
- what to do when i can't get enough current

|                     | USB connected                      | USB disconnected   |
| ------------------- | ---------------------------------- | ------------------ |
| **Battery charged** | Power with USB                     | Power with battery |
| **Battery empty**   | Power with USB, and charge battery | Do nothing         |

### Priority

1. USB (power jack and charge battery)
2. Jack (charge battery)
3. Battery (power jack)

## Notes

> The device uses a ratiometric architecture that can minimize error from VCC tolerance when the external analog-to-digital converter (ADC) uses the same VCC for the reference.

> TI recommends proper power-supply sequencing for all CMOS devices. Do not exceed the absolute maximum ratings, because stresses beyond the listed ratings can cause permanent damage to the device. Always sequence VCC on first, followed by NO or COM.

<iframe data-testid="embed-iframe" style="border-radius:12px" src="https://open.spotify.com/embed/album/1xQGeKOIMZrPBUlDJuqZGQ?utm_source=generator" width="100%" height="352" frameBorder="0" allowfullscreen="" allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture" loading="lazy"></iframe>
