## SET\_NOISE\_GATE\_ENABLED

Enable/Disable Noise Gate for a Channel.

### Name
`SET_NOISE_GATE_ENABLED (roomId: Long, channelId: Int, enabled: Boolean)`


| Parameter | Type | Description                     |
| --------- | ---- | ------------------------------- |
| roomId    | Long | ID value of the room.           |
| channeld  | INT  | ID value of the channel.        |
| enabled   | Bool | Noise Gate enabled state (t/f). |


### Example
`SET_NOISE_GATE_ENABLED({enabled = True, channelId = 2, roomId:  7977})`
