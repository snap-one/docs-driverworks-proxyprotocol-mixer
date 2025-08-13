## SET\_EQ\_BAND\_Q\_LEVEL

**SET EQ BAND Q LEVEL**

Sets the EQ Band Q for a Channel.

### Name
`SET_EQ_BAND_Q_LEVEL(roomId: Long, channelId: Int, bandId: Int, level: Float)`


| Parameter | Type  | Description              |
| --------- | ----- | ------------------------ |
| roomId    | Long  | ID value of the room.    |
| channeld  | INT   | ID value of the channel. |
| bandId    | INT   | ID value of the EQ band. |
| level     | Float | Q Level value.           |


### Example
`SET_EQ_BAND_Q_LEVEL({channelId = 2, bandId = 1, level = 3, roomId:  7977})`


