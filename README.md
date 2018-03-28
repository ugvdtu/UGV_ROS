# UGV_ROS
### Steering commands can be sent through the messages of type SteerCmd
It contains the two fields - `float32 value` and `uint8 cmdType`. `cmdType` describes the type of command. It can be either of following three values, and the `value` field takes meaning accordingly:
* `0`: This command tells the bot to move forward. The `value` field is interpreted as the velocity with which the vehicle moves.
* `1`: This command tells the bot to make a point turn (ie about the center axis). The `value` field is interpreted as the angle with which to rotate.
* `2`: This command tells the bot to make a swing turn (ie about a corner axis). The `value` field is interpreted the same as `1`.

Note: Positive values of angle mean right turn while negative values of angle means left turn.
