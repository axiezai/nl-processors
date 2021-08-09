Datasets:
---

The datasets might be too big for Github repos to host, so I'm putting links here instead, but can potentially save smaller data chunks here for testing.

 - OpenNeuro Study Forrest: https://openneuro.org/datasets/ds000113/versions/1.3.0
    - Eye-gaze metadata file: https://openneuro.org/datasets/ds000113/versions/1.3.0/file-display/recording-eyegaze_physio.json
    - Movie segments cut at roughly 15min segments, scene cuts were at:
        - 22320
        - 48014
        - 70175
        - 97461
        - 123462
        - 149402
        - 178109
        - 194803
    - Frames:
        - `fps` = 25
        - `fadeoutframes` = 100
        - `fadeinframes` = 25
    - In frame/ out frame? 
        - ```
            in_segments = (
                (0, 32312),
                (36349, 57798),
                (58470, 85997),
                (89293, 117351),
                (120616, 141457),
                (145869, 152269),
                (154244, 194792)
            )
            ```

### Files:
 - `studyforrest_german_transcript.csv` - This transcript contains all information on the audio-movie content that cannot be inferred from the DVD release — in a plain text, comma-separated-value table. Start and end time stamp, as well as the spoken text are provided for each continuous audio description segment.