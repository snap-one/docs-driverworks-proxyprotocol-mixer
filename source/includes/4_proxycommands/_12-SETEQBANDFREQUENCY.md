## SET\_EQ\_BAND\_FRQUENCY

Sets the EQ Band Center Frequency for a Channel.


### Name
`SET_EQ_BAND_FREQUENCY(roomId: Long, channelId: Int, bandId: Int, frequency: Int)`


| Parameter | Type | Description              |
| --------- | ---- | ------------------------ |
| roomId    | Long | ID value of the room.    |
| channeld  | INT  | ID value of the channel. |
| bandId    | INT  | ID value of the EQ band. |
| frequency | INT  | Center frequency value.  |


### Example
`SET_EQ_BAND_FREQUENCY({channelId = 2, bandId = 1, frequency = 200, roomId:  7977})`


