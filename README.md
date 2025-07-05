# RV1126 SDK Bundle

This repository contains external resources and prebuilt packages required by the RV1126 SDK, making it easy for users to download and restore from GitHub Releases.

This bundle originates from [Firefly](https://en.t-firefly.com/), a China company that publicly hosts these repositories on [Firefly Linux GitLab](https://gitlab.com/firefly-linux).
To reduce disk space usage and shorten the sync time when syncing the full repository, several large repositories have been separated out into this independent package.

---

## Download Location

Please download the corresponding compressed split files from the [Releases page](https://github.com/uwingstech/rv1126-bundle/releases) of this repository.

---

## Extraction Instructions

After downloading, please extract the files to your desired folders using the commands below.

---

### 1. buildroot/dl

Files to download:

- [rv1126-buildroot-dl.part00.tar.zstd](https://github.com/uwingstech/rv1126-bundle/releases/download/v2.5.5g-sdk-bundle/rv1126-buildroot-dl.part00.tar.zstd), sha256: a0a212536b75d8e8389450fe15f721d5a42662cc1b905098d501a7c0a7ab6656
- [rv1126-buildroot-dl.part01.tar.zstd](https://github.com/uwingstech/rv1126-bundle/releases/download/v2.5.5g-sdk-bundle/rv1126-buildroot-dl.part01.tar.zstd), sha256: 6b36df465af741bb323651b26c2b811646bee329d0659d53b25900fff517f6f2
- [rv1126-buildroot-dl.part02.tar.zstd](https://github.com/uwingstech/rv1126-bundle/releases/download/v2.5.5g-sdk-bundle/rv1126-buildroot-dl.part02.tar.zstd), sha256: d1e0c5a256a9b1665ef50febc35cb0b834d5cc91f50bb42eae381b5b4c46d6d5
- [rv1126-buildroot-dl.part03.tar.zstd](https://github.com/uwingstech/rv1126-bundle/releases/download/v2.5.5g-sdk-bundle/rv1126-buildroot-dl.part03.tar.zstd), sha256: dc1e721447b3e36bf82e067b33b8061084e034b0b0e2c368df4ada345d101b5c

Extraction command:

```
cat rv1126-buildroot-dl.part*.tar.zstd | \
    tar -I zstd -xvf - -C <your buildroot/dl folder>
```


Replace `<your buildroot-dl folder>` with the actual target directory.

---

### 2. external/rockx

Files to download:

- [rv1126-external-rockx.part00.tar.zstd](https://github.com/uwingstech/rv1126-bundle/releases/download/v2.5.5g-sdk-bundle/rv1126-external-rockx.part00.tar.zstd), sha256: 99ae69eb341cd04e6e3e2fad56286c8721019cf05ea520d1e45138eaa10489b0
- [rv1126-external-rockx.part01.tar.zstd](https://github.com/uwingstech/rv1126-bundle/releases/download/v2.5.5g-sdk-bundle/rv1126-external-rockx.part01.tar.zstd), sha256: 7252e7850be22b1d806f35ab62000b2b1711d6c7a5118da3da8dd999f679f1a7

Extraction command:

```
cat rv1126-external-rockx.part*.tar.zstd | \
    tar -I zstd -xvf - -C <your external/rockx folder>
```


---

### 3. external/rknn-toolkit

Files to download:

- [rv1126-external-rknn-toolkit.part00.tar.zstd](https://github.com/uwingstech/rv1126-bundle/releases/download/v2.5.5g-sdk-bundle/rv1126-external-rknn-toolkit.part00.tar.zstd), sha256: a2a492c5c770ca41fe26a41467dcdd4d7739e329663408329632706742c9bae0
- [rv1126-external-rknn-toolkit.part01.tar.zstd](https://github.com/uwingstech/rv1126-bundle/releases/download/v2.5.5g-sdk-bundle/rv1126-external-rknn-toolkit.part01.tar.zstd), sha256: fe4f1625e915ed4a6a27f865f5c9f9ddac43b09c8e19f5f7a267f285d593ca71

Extraction command:

```
cat rv1126-external-rknn-toolkit.part*.tar.zstd | \
    tar -I zstd -xvf - -C <your external/rknn-toolkit folder>
```


---

### 4. external/camera_engine_rkaiq

Files to download:

- [rv1126-external-camera_engine_rkaiq.tar.zstd](https://github.com/uwingstech/rv1126-bundle/releases/download/v2.5.5g-sdk-bundle/rv1126-external-camera_engine_rkaiq.tar.zstd), sha256: 1db4fc2b46b37d302da575e0239b4480a49bae52473ac91f2dc182f05334eb43

Extraction command:

```
tar -I zstd -xvf rv1126-external-camera_engine_rkaiq.tar.zstd \
    -C <your external/camera_engine_rkaiq folder>
```

---

### 5. prebuilts/gcc/linux-x86/arm/gcc-linaro-6.3.1-2017.05-x86_64_arm-linux-gnueabihf

Files to download:

- [prebuilts-gcc-linaro-6.3.1.tar.zstd](https://github.com/uwingstech/rv1126-bundle/releases/download/v2.5.5g-sdk-bundle/prebuilts-gcc-linaro-6.3.1.tar.zstd), sha256: d8a7047d136b492b002d0cb7af223ee59489b21d8c07cd647dd6baefdb321e51

Extraction command:

```
tar -I zstd -xvf prebuilts-gcc-linaro-6.3.1.part*.tar.zstd -C \
    <your prebuilts/gcc/linux-x86/arm/gcc-linaro-6.3.1-2017.05-x86_64_arm-linux-gnueabihf folder>
```

---

### 6. prebuilts/gcc/linux-x86/arm/gcc-arm-8.3-2019.03-x86_64-arm-linux-gnueabihf

Files to download:

- [prebuilts-gcc-arm-8.3.tar.zstd](https://github.com/uwingstech/rv1126-bundle/releases/download/v2.5.5g-sdk-bundle/prebuilts-gcc-arm-8.3.tar.zstd), sha256: 449de113f978cfa6c1972818fa1bf505b76e740e349e32e42b022bf284030f5d

Extraction command:

```
tar -I zstd -xvf prebuilts-gcc-arm-8.3.tar.zstd -C \
    <your prebuilts/gcc/linux-x86/arm/gcc-arm-8.3-2019.03-x86_64-arm-linux-gnueabihf folder>
```

---

## Notes

- Please ensure your system has `tar` with `zstd` support (`tar` version supporting `-I zstd`) and the `zstd` decompression tool installed.
- Replace `<your ... folder>` with the actual directory where you want to extract the files.
- Make sure the target directories exist and have enough disk space before extraction.

