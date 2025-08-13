## SET\_NOISE\_GATE\_COMPONENT\_VALUE

Sets the Value of a Noise Gate Element for a Channel.


### Name
`SET_NOISE_GATE_COMPONENT_VALUE(roomId: Long, channelId: Int, key: String, value: Float)`

| Parameter | Type  | Description               |
| --------- | ----- | ------------------------- |
| roomId    | Long  | ID value of the room.     |
| channeld  | INT   | ID value of the channel.  |
| key       | STR   | ID value of the key.      |
| value     | Float | Noise Gate Element value. |


### Example
`SET_NOISE_GATE_COMPONENT_VALUE({channelId = 2, key = 'release', value = 250, roomId:  7977})`


