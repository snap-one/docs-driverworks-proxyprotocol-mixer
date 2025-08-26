## SET\_EQ\_BAND\_ENABLED

Enable/Disable an EQ Band for a Channel.

### Name
`SET_EQ_BAND_ENABLED(roomId: Long, channelId: Int, bandId: Int, enabled: Boolean)`


| Parameter | Type | Description                  |
| --------- | ---- | ---------------------------- |
| roomId    | Long | ID value of the room.        |
| channeld  | INT  | ID value of the channel.     |
| bandId    | INT  | ID value of the EQ band.     |
| enabled   | Bool | EQ Band enabled state (t/f). |


### Example
`SET_EQ_BAND_ENABLED({channelId = 2, bandId = 1, enabled = True, roomId:  7977})`

