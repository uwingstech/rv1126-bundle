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

- rv1126-buildroot-dl.part00.tar.zstd
- rv1126-buildroot-dl.part01.tar.zstd
- rv1126-buildroot-dl.part02.tar.zstd
- rv1126-buildroot-dl.part03.tar.zstd

Extraction command:

```
cat rv1126-buildroot-dl.part*.tar.zstd | \
    tar -I zstd -xvf - -C <your buildroot/dl folder>
```


Replace `<your buildroot-dl folder>` with the actual target directory.

---

### 2. external/rockx

Files to download:

- rv1126-external-rockx.part00.tar.zstd
- rv1126-external-rockx.part01.tar.zstd
- rv1126-external-rockx.part02.tar.zstd

Extraction command:

```
cat rv1126-external-rockx.part*.tar.zstd | \
    tar -I zstd -xvf - -C <your external/rockx folder>
```


---

### 3. external/rknn-toolkit

Files to download:

- rv1126-external-rknn-toolkit.part00.tar.zstd
- rv1126-external-rknn-toolkit.part01.tar.zstd

Extraction command:

```
cat rv1126-external-rknn-toolkit.part*.tar.zstd | \
    tar -I zstd -xvf - -C <your external/rknn-toolkit folder>
```


---

### 4. external/camera_engine_rkaiq

Files to download:

- rv1126-external-camera_engine_rkaiq.part00.tar.zstd
- rv1126-external-camera_engine_rkaiq.part01.tar.zstd

Extraction command:

```
cat rv1126-external-camera_engine_rkaiq.part*.tar.zstd | \
    tar -I zstd -xvf - -C <your external/camera_engine_rkaiq folder>
```

---

### 5. prebuilts/gcc/linux-x86/arm/gcc-linaro-6.3.1-2017.05-x86_64_arm-linux-gnueabihf

Files to download:

- rv1126-prebuilts-gcc-linaro-6.3.1.part00.tar.zstd
- rv1126-prebuilts-gcc-linaro-6.3.1.part01.tar.zstd

Extraction command:

```
cat rv1126-prebuilts-gcc-linaro-6.3.1.part*.tar.zstd | \
    tar -I zstd -xvf - -C \
    <your prebuilts/gcc/linux-x86/arm/gcc-linaro-6.3.1-2017.05-x86_64_arm-linux-gnueabihf folder>
```

---

### 6. prebuilts/gcc/linux-x86/arm/gcc-arm-8.3-2019.03-x86_64-arm-linux-gnueabihf

Files to download:

- rv1126-prebuilts-gcc-arm-8.3.part00.tar.zstd
- rv1126-prebuilts-gcc-arm-8.3.part01.tar.zstd

Extraction command:

```
cat rv1126-prebuilts-gcc-arm-8.3.part*.tar.zstd | \
    tar -I zstd -xvf - -C \
    <your prebuilts/gcc/linux-x86/arm/gcc-arm-8.3-2019.03-x86_64-arm-linux-gnueabihf folder>
```

---

## Notes

- Please ensure your system has `tar` with `zstd` support (`tar` version supporting `-I zstd`) and the `zstd` decompression tool installed.
- Replace `<your ... folder>` with the actual directory where you want to extract the files.
- Make sure the target directories exist and have enough disk space before extraction.

