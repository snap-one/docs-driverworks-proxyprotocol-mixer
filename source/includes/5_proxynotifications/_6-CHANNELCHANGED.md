## CHANNEL\_CHANGED

Notification of change in any Channel Parameter.


### Name
`CHANNEL_CHANGED(MIXER_CHANNEL: Table)`


| Parameter | Type | Description                                                   |
| --------- | ---- | ------------------------------------------------------------- |
| Table     | STR  | Param table encoded as a JSON string param  of mixer channel. |

### Example
In this example, Channel 1 Input Level has changed to -7.

```json
{"RoomId":7977,"id":1,"input_level":{"value":-7}}
```

In this example, The Gain of Band 1 of the EQ in Channel 1 has changed to 7.9.

```json
{"RoomId":7856,"eq":{"bands":[{"gain":{"value":7.9000000000000004},"id":1}]},"id":1}
```


