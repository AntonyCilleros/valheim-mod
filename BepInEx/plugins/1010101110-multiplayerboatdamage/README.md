# multiplayerboatdamage (bugfix)

This mod runs on a client. Whoever owns the boat object simulates the boat water impact damage. If you are on a server and someone else owns the boat object it will still take damage if they don't have the mod installed. So tell all your friends to install this as well!

If you are alone or own the boat object then this should work great to stop the constant boat damage.

There is no server side fix for this issue because the water impact code is run on the client using local variables. 

# install

i would suggest installing this easily with r2modman

# code

```Cs
Ship.m_minWaterImpactForce = 100f;
```