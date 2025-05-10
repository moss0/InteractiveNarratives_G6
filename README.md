# InteractiveNarratives_G6
 The interactive narratives project by group 6.

GitHub repository: https://github.com/moss0/InteractiveNarratives_G6

## Development

### Third person shooting

I started off with the third person aim and shoot mechanics, deciding to make an aiming mode upon holding down Secondary fire (right mouse button.)

After watching a video, (LINK LINK LINK) I learned that doing this in Event tick was not the proper way to implement this feature as it will cause performance problems when the project scales up in size. I decided to use a looping timer connected to an event that gets unpaused and paused upon pressing and releasing the mouse, respectively.

### AI NPCs

I decided to migrate my previous AI from the Client brief project in order to improve old code and add new features to save time.

#### Patrolling
Initially the increment code was kept inside of BP_PatrolRoute until I realised it does not support multiple NPC's using the same patrol route. I decided to move the code to within BP_NPC_Base so that way every NPC using the route has its own count of what spline index it is at, what direction along the spline to move, etc.
