# Results

## Test Cases — All 10 Passed ✅

| Test | Scenario | Result |
|------|----------|--------|
| 1 | Hand tracking | Hand detected with landmarks |
| 2 | Hand tracking by gestures | Index finger tracked with FPS |
| 3 | Volume control | Volume adjusted by hand gestures |
| 4 | Increase volume to maximum | Volume reached 100% |
| 5 | Mute command | Volume decreased to minimum |
| 6 | Volume control on local audio files | Audio controlled correctly |
| 7 | Volume control on online audio | Works on streaming audio |
| 8 | Volume control on online videos | Works on online video audio |
| 9 | Volume control on custom playlist | Songs controlled via gestures |
| 10 | Parallel system volume check | Volume displayed and controlled in parallel |

## Key Observations

- Real-time FPS maintained between 20–36 during testing
- Distance between thumb (landmark 4) and index finger (landmark 8) accurately mapped to volume range 0–100%
- Volume bar displayed at top-right corner updated in real time
- System volume and gesture volume bar ran in parallel correctly
- All 10 test cases passed with no failures
