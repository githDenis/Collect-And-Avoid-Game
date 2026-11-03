Engine version: 5.7



Changed character movement parameters:

MaxWalkSpeed: 600 -> 650

GravityScale: 1 -> 1.5

JumpZVelocity: 420 -> 450



Why is the cast check needed when you pick up a coin?

The cast is needed because EventActorBeginOverlap returns overlapped actor and we need to cast it to BP\_Here. If overlapped actor is BP\_Hero

Cast will return reference at this object. If It's not Cast will be failed



Why is the Update Score function called in event?

Update score function isn't called in Tick function because this is bad for perfomance. So Update function is called when the player picks up a coin.

