## SET\_DE\_ESSER\_COMPONENT\_VALUE

Sets the Value of a De-Esser Element for a Channel.

### Name
`SET_DE_ESSER_COMPONENT_VALUE(roomId: Long, channelId: Int, key: String, value: Float)`

| Parameter | Type  | Description              |
| --------- | ----- | ------------------------ |
| roomId    | Long  | ID value of the room.    |
| channeld  | INT   | ID value of the channel. |
| key       | STR   | ID value of the key.     |
| value     | Float | De-esser Element value.  |


### Example
`SET_DE_ESSER_COMPONENT_VALUE({channelId = 2, key = 'reduction', value = -5, roomId:  7977})`

