# Formato messaggio FtD


## Distrazione visuale - AITEK
```json
// TOPIC: ???
{
    "time": 123456, 
    "eyesOffRoad": 0, // Bool {0, 1}
    "eyesOffRoad_confidence": 0.0, // Float [0..1]
    "eyesOffRoad_pred_1s": 0.0, // Float [0..1]
}
```

## Distrazione cognitiva - Torino
```json
// TOPIC: NP_UNITO_DCDC
{
    "time": 123456, 
    "cognitive_distraction": 1, // Bool {0, 1}
    "cognitive_distraction_confidence": 0.0, // Float [0..1]
    "cognitive_distraction_pred_1s": 0.0 // Float [0..1]
}
```

## Emozioni - Emoji
```json
// TOPIC: Emotions
{
    "person0" : {
        "predominant" : "0",

        /* Somma emozioni = 1 */
        "neutral":"0.0008",
        "happiness": "0.0097",
        "surprise":"0.0106",
        "sadness": "0.0176",
        "anger": "0.7015",
        "disgust": "0.1255",
        "fear": "0.1343",

        "engagement": "4.4877",
        "valence": "0.0154492"
    }
}
```

## Arousal - UniPR
```json
// TOPIC: NP_UNIPR_AROUSAL
{
    "arousal": 0.0 // Float [0..1]
}
```

## Telemetria Simulatore - ReLab
```json
// TOPIC: NP_RELAB_VD
{
    /* altre informazioni */
    
    "x": 0 // Int

}
```