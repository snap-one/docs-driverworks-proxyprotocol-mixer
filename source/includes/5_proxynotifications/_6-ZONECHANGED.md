## ZONE\_CHANGED

Notification of change in any Zone Parameter

### Name
`ZONE_CHANGED(MIXER_ZONE: Table)`


| Parameter | Type | Description                                                  |
| --------- | ---- | ------------------------------------------------------------ |
| Table     | STR  | Param table encoded as a JSON string param  of a mixer zone. |


### Example
In this example, Source 2 has been selected in Zone 1.

```json
{"RoomId":7977,"id":1,"source":2,"sourceConnId":3002}
```

In this example, the Gain in Zone 1 has changed to -22.

```json
{"RoomId":7977,"gain":-22,"id":1}
```


