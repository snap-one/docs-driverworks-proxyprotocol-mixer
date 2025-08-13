## SET\_ROUTING 

Routes a Channel or a Mix to a Zone.

### Name
`SET_ROUTING ({ZONE_ID: Int, CHANNEL_ID: Int})`


| Parameter | Type | Description              |
| --------- | ---- | ------------------------ |
| zoneId    | INT  | ID value of the zone.    |
| channelId | INT  | ID value of the channel. |


### Example
In this example, the Channel 1 is Routed to Zone 1.

`SET_ROUTING ({ZONE_ID = 1, CHANNEL_ID = 1})`


