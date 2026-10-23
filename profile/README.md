# fruity-aospa

Unofficial Paranoid Android (AOSPA) builds and trees for the Nothing Phone (3a), codename `asteroids`
(Qualcomm SM7635, kernel 6.6, Android 17).

## Where things are

Everything is tracked by [`manifest`](https://github.com/fruity-aospa/manifest), branch `asteroids`.

```
repo init -u https://github.com/fruity-aospa/manifest -b asteroids
repo sync -c
```

| Repository | Contents |
|---|---|
| `android_device_nothing_asteroids` | Device tree |
| `proprietary_vendor_nothing_asteroids` | Vendor blobs (stock `C5.0-260915-2123`) |
| `android_hardware_nothing` | Glyph, vibrator and fingerprint |
| `android_kernel_nothing_sm7635` | Kernel, with the `-modules` and `-devicetrees` repositories |
| `android_hardware_qcom_audio-ar` and the other audio repositories | AudioReach HALs, including `st-hal-ar` for the sound trigger HAL |
| `android_device_qcom_common`, `android_vendor_aospa` | Shared Qualcomm and AOSPA components |

Forks keep their upstream history. The kernel carries Qualcomm (CLO) and Google ACK changes under their
original authors, and ported commits keep the upstream author with a link to the source commit.

## AI assistance

The work in this organization is developed with AI assistance. AI tools are used for log analysis,
code review, drafting changes and writing commit messages. The maintainer reviews the changes and does
the builds and device testing.
