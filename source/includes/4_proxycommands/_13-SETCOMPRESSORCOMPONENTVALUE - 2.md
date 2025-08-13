## SET\_COMPRESSOR\_COMPONENT\_VALUE

Sets the Value of a Compressor Element for a Channel.


### Name
`SET_COMPRESSOR_COMPONENT_VALUE(roomId: Long, channelId: Int, key: String, value: Float)`


| Parameter | Type  | Description               |
| --------- | ----- | ------------------------- |
| roomId    | Long  | ID value of the room.     |
| channeld  | INT   | ID value of the channel.  |
| key       | STR   | ID value of the key.      |
| value     | Float | Compressor Element value. |


### Example
`SET_COMPRESSOR_COMPONENT_VALUE({channelId = 2, key = 'threshold', value = -10, roomId:  7977})`

