## SET\_CHANNEL

Sets any element that is declared in the JSON Channel structure. The parameter 'id' is required, the other parameters dictate the element to be set.


### Name
`SET_CHANNEL (param: String)`


| Parameter | Type   | Description |
| --------- | ------ | ----------- |
| param     | STRING | JSON String |


### Example
In this example, the EQ for Channel 1 is being disabled.

`SET_CHANNEL({param = '{"RoomId":7856,"eq":{"enabled":false},"id":1}}')`
