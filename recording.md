# Recording

My recording settings

## OBS-Studio

### Output

- **Output Mode:** Advanced

#### Recording

##### Recording Settings

> I only changed "Recording" tab, no other was changed.

- **Type**: Standard
- **Recording Format**: Matroska Video (`.mkv`)[^1]
- **Audio Encoder**: FFmpeg PCM (32-bit float)

##### Encoder Settings

- **Rate Control**: Constant QP
- **Constant QP**: `20`
- **Keyframe Interval**: `2s`
- **Preset**: P5: Slow (Good Quality)[^2]
- **Tuning**: High Quality[^2]
- **Multipass Mode**: Single Pass[^2]
- **B-Frames**: `1`

### Audio

- **Sample Rate:** `48 KHz`
- **Make sure** _"Global Audio Devices"_ is properly setup (so OBS-Studio knows which devices to use)

### Video

- **Base (Canvas) Resolution**: `1920`x`1080`
- Output (Scaled) Resolution: `1920`x`1080`
- **Common FPS Values**: `60`

### Advanced

- [X] Automatically remux to `.mp4`

## Notes

- [^1]: If you choose a different format and it uses `.mp4`, [disable auto. remux](#advanced)
- [^2]: This settings vastly vary from system to system. You may need to turn it down (or up if you got a beefy device)
