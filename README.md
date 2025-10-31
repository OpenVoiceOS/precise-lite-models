# Precise Lite Models

Free models for usage with precise-lite

## Related repos

- **NEW** - [ovos-ww-plugin-precise-onnx](https://github.com/TigreGotico/ovos-ww-plugin-precise-onnx) - OVOS plugin for precise-lite  (.onnx models)
- [ovos-ww-plugin-precise-lite](https://github.com/OpenVoiceOS/ovos-ww-plugin-precise-lite) - OVOS plugin for precise-lite (.tflite models)
- [precise-lite-trainer](https://github.com/OpenVoiceOS/precise-lite-trainer) - train/convert models with this
- [precise-lite-runner](https://github.com/OpenVoiceOS/precise_lite_runner) - standalone precise tflite model runner
- [precise-community-data](https://github.com/MycroftAI/precise-community-data) - Community data

## Training

- [el-tocino/localcroft/precise](https://github.com/el-tocino/localcroft/blob/master/precise/Precise.md)
- [secret_sauce_ai/Wake-Word-Project](https://github.com/secretsauceai/secret_sauce_ai/wiki/Wake-Word-Project)

## Model Info

| model           | ww dataset                               | not-ww datasets                                    | epochs | batch size | sensitivity | dopout | notes                                                                                                            |
|-----------------|------------------------------------------|----------------------------------------------------|--------|------------|-------------|--------|------------------------------------------------------------------------------------------------------------------|
| hey_mycroft_mk1 | proprietary MycroftAI (user opt-in data) | pdsounds (?)                                       | 6000   | 5000       | 0.8         | 0.2    | model for the Mark I - data collected via previous pocketsphinx wakeword and tagged via crowdsourcing in a WebUI |
| hey_mycroft     | proprietary MycroftAI (user opt-in data) |                                                    | 6000   | 5000       | 0.8         | 0.2    | model for the Mark II - pitch classified (with 89% confidence level) and balanced version of the original set    |
| christopher     | proprietary MycroftAI                    |                                                    |        |            |             |        | unannounced but uploaded to MycroftAI github                                                                     |
| cough           | proprietary MycroftAI                    |                                                    |        |            |             |        | unannounced but uploaded to MycroftAI github, probably the result of their SickWeather collaboration             |
| sheila          | google-speech-commands                   | synthetic data + pdsounds + proprietary dataset    | 1000   | 3000       | 0.1         |        |                                                                                                                  |
| marvin          | google-speech-commands                   | synthetic data + pdsounds + proprietary dataset    | 1000   | 100        | 0.1         |        |                                                                                                                  |
| android         | proprietary dataset                      | synthetic data + pdsounds + google-speech-commands |        |            |             |        | dataset known to contain mislabeled samples                                                                      |
| hey_robin       | proprietary dataset                      | synthetic data + pdsounds + google-speech-commands | 1000   | 3000       | 0.2         |        |                                                                                                                  |
| hey_firefox     | probably common voice                    | pdsounds + google-speech-commands + ?              |        |            |             |        | no longer available, dataset was linked in castorini/howl repository                                             |
| hey_moxie       |                                          | pdsounds + google-speech-commands + ?              |        |            |             |        |                                                                                                                  |
| hey_scout       |                                          | pdsounds + google-speech-commands + ?              |        |            |             |        |                                                                                                                  |
| hey_chatterbox  | mycroft community dataset                |                                                    |        |            |             |        |                                                                                                                  |
| computer        | mycroft community dataset                |                                                    |        |            |             |        | wrong model uploaded or not trained long enough, avoid                                                           |
| hey_k9          | mycroft community dataset                |                                                    |        |            |             |        |                                                                                                                  |