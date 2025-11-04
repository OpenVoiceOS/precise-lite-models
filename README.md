# Precise Lite Models

Free models for usage with precise-lite

## Related repos

- **NEW** - [ovos-ww-plugin-precise-onnx](https://github.com/TigreGotico/ovos-ww-plugin-precise-onnx) - OVOS plugin for
  precise-lite  (.onnx models)
- [ovos-ww-plugin-precise-lite](https://github.com/OpenVoiceOS/ovos-ww-plugin-precise-lite) - OVOS plugin for
  precise-lite (.tflite models)
- [precise-lite-trainer](https://github.com/OpenVoiceOS/precise-lite-trainer) - train/convert models with this
- [precise-lite-runner](https://github.com/OpenVoiceOS/precise_lite_runner) - standalone precise tflite model runner
- [precise-community-data](https://github.com/MycroftAI/precise-community-data) - Community data

## Training

- [el-tocino/localcroft/precise](https://github.com/el-tocino/localcroft/blob/master/precise/Precise.md)
- [secret_sauce_ai/Wake-Word-Project](https://github.com/secretsauceai/secret_sauce_ai/wiki/Wake-Word-Project)

## Model Info

| model            | ww dataset                               | not-ww datasets                                                                | epochs | batch size | sensitivity | dopout | notes                                                                                                                                                     |
|------------------|------------------------------------------|--------------------------------------------------------------------------------|--------|------------|-------------|--------|-----------------------------------------------------------------------------------------------------------------------------------------------------------|
| hey_mycroft_mk1  | proprietary MycroftAI (user opt-in data) | user opt-in data (?) + hundreds of hours of youtube audio                      | 6000   | 5000       | 0.8         | 0.2    | model for the Mark I - 114,000 'hey mycroft' wake word samples, data collected via previous pocketsphinx wakeword and tagged via crowdsourcing in a WebUI |
| hey_mycroft      | proprietary MycroftAI (user opt-in data) | 68,000 samples subset of hey_mycroft_mk1 dataset                               | 6000   | 5000       | 0.8         | 0.2    | model for the Mark II -  balanced version of the original set, classified samples into high/low pitched (34,000 samples each).                            |
| christopher      | proprietary MycroftAI                    | user opt-in data (?) + hundreds of hours of youtube audio (?)                  |        |            |             |        | unannounced but uploaded to MycroftAI github                                                                                                              |
| cough            | proprietary MycroftAI                    | hundreds of hours of youtube audio (?)                                         |        |            |             |        | unannounced but uploaded to MycroftAI github, probably the result of their SickWeather collaboration                                                      |
| sheila           | google-speech-commands                   | synthetic data + pdsounds + proprietary dataset + mycroft community dataset    | 1000   | 3000       | 0.1         |        |                                                                                                                                                           |
| marvin           | google-speech-commands                   | synthetic data + pdsounds + proprietary dataset + mycroft community dataset    | 1000   | 100        | 0.1         |        |                                                                                                                                                           |
| android          | proprietary dataset                      | synthetic data + pdsounds + google-speech-commands + mycroft community dataset |        |            |             |        | dataset known to contain mislabeled samples                                                                                                               |
| hey_robin        | proprietary dataset                      | synthetic data + pdsounds + google-speech-commands + mycroft community dataset | 1000   | 3000       | 0.2         |        |                                                                                                                                                           |
| hey_firefox      | probably common voice (?)                | pdsounds + google-speech-commands + mycroft community dataset + ?              |        |            |             |        | no longer available, dataset was linked in castorini/howl repository                                                                                      |
| hey_moxie        | ?                                        | pdsounds + google-speech-commands + mycroft community dataset + ?              |        |            |             |        |                                                                                                                                                           |
| hey_scout        | ?                                        | pdsounds + google-speech-commands + mycroft community dataset + ?              |        |            |             |        |                                                                                                                                                           |
| hey_chatterbox   | mycroft community dataset                | pdsounds + google-speech-commands + mycroft community dataset + ?              |        |            |             |        |                                                                                                                                                           |
| computer         | mycroft community dataset                | pdsounds + google-speech-commands + mycroft community dataset + ?              |        |            |             |        | 100 steps, .9938, 52 training words, 5 test                                                                                                               |
| hey_k9           | mycroft community dataset                | pdsounds + google-speech-commands + mycroft community dataset + ?              |        |            |             |        |                                                                                                                                                           |
| athena           | mycroft community dataset                | pdsounds + google-speech-commands + mycroft community dataset + ?              |        |            |             |        |                                                                                                                                                           |
| ey_ordenador_0.2 | mycroft community dataset                | pdsounds + google-speech-commands + mycroft community dataset + ?              |        |            |             |        | 250 steps, 44 training words, 5 test                                                                                                                      |
| ey_ordenador_0.3 | mycroft community dataset                | pdsounds + google-speech-commands + mycroft community dataset + ?              |        |            |             |        | 50 steps, 44 training words, 5 test                                                                                                                       |