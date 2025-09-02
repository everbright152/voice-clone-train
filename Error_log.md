# Error Log Document


# 1). 
Dependencies confusion — didn’t know why I needed things like ffmpeg-python, whisper, soundfile, datasets. Also used imports like os, json, subprocess, uuid, torch, glob, Path without fully knowing their purpose.

# 2).
Tried from google.collab import files → typo! (should be colab not collab) → got ModuleNotFoundError.

# 3).
Didn’t know about VRAM, Orpheous, CSM_1B, TTS. Also wasn’t familiar with Google Colab usage.

# 4).
Struggled with setting up file paths for uploads.

# 5).
Instructor used 6 YouTube files, I only used 1 uploaded file → had to rewrite code for single file, no loop → caused issues.

# 6).
No idea about batch processing & transcribing at first.

# 7).
CalledProcessError while cleaning audio (FFmpeg failures). Had to check file existence, filter syntax, capture error output.

# 8).
Tried running FFmpeg outside function → NameError (because src wasn’t defined).

# 9).
Another CalledProcessError while extracting a clip from Voice_Cloning_Audio_Raw_clean.wav even though file was there. Turned out to be path formatting.

# 10).
Got stuck figuring out purpose of temp_original_clip_path + some other functions.

# 11).
subprocess + ffprobe script failed to extract duration from .mp3 → path issues again.

# 12).
TypeError with datasets.Audio: couldn’t cast array properly (list<item: list<item: float>> issue).

# 13).
'list' object has no attribute 'T' error.

# 14).
Double nesting problem: {'array': array([array({...})])}.

# 15).
Waveform shape issues: expected (samples,) but got () or (1,).

# 16).
ZeroDivisionError during push: some rows had sampling_rate = 0 or empty waveforms.

# 17).
ArrowInvalid: Only 1D arrays accepted.

# 18).
Malformed audio in clip_rows: "audio" was raw tensor without conversion.

# 19).
Too many skipped rows → chunks were scalar/empty because of slicing mistakes.

# 20).
Dataset didn’t load correctly into Hugging Face.

# 21).
torchcodec installation error.
