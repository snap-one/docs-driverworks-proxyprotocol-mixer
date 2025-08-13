## SET\_EQ\_BAND\_GAIN\_LEVEL

Sets the EQ Band gain level for a Channel.


### Name
`SET_EQ_BAND_GAIN_LEVEL(roomId: Long, channelId: Int, bandId: Int, level: Float)`


| Parameter | Type  | Description              |
| --------- | ----- | ------------------------ |
| roomId    | Long  | ID value of the room.    |
| channeld  | INT   | ID value of the channel. |
| bandId    | INT   | ID value of the EQ band. |
| level     | Float | Gain Level value.        |


### Example
`SET_EQ_BAND_GAIN_LEVEL({channelId = 2, bandId = 1, level = 3, roomId:  7977})`

