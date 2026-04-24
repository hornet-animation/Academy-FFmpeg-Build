# Build Academy FFmpeg toolchain

Builds ffmpeg with OCIO support and VFX reference platform codecs from [AcademySoftwareFoundation/EncodingGuidelines](https://github.com/AcademySoftwareFoundation/EncodingGuidelines) for Linux (Rocky 9) and Windows (MinGW64).

actions-only workflow using github hosted workers on both platforms, pushing to `Releases`
## Usage

Go to the [Actions tab](../../actions), select **build-ffmpeg**, click **Run workflow**.

Each run builds the latest `main` of the upstream repo and publishes a release tagged `build-YYYYMMDD-<shortsha>` with the binaries attached.

## Outputs

- `ffmpeg-linux-x86_64.zip` — Rocky 9 / RHEL 9 build
- `ffmpeg-windows-x86_64.zip` — Windows MinGW64 build
