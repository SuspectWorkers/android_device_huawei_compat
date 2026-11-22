# android_device_huawei_compat

Huawei Kirin 960 legacy HAL and shim compatibility tree adapted from `Trijal08/android_device_huawei_compat` (`android@13`) for clean **AOSP 13** builds.

## AOSP 13 Adaptations

- Added `libui_shim.cpp` (`android::Fence::~Fence()`, `GraphicBuffer::lock`, `GraphicBufferMapper::lock`) for camera HAL compatibility (`libcamera_algo.so`).
- Removed unused Lineage-specific HAL modules (`livedisplay`, `touch`) and unused shims (`libshim_emcom`, `libshim_hwcam`, `guivnd`) that do not exist in pure AOSP 13.
