# BMW ConnectedDrive lets me control my returned rental car (Sixt)

**Posted by derturm666 on 2025-06-17**

Last week, I rented a BMW from Sixt in Italy. The default rental driver profile had Bluetooth disabled, so I created my own BMW ID, paired it with the vehicle, removed the original profile, and even triggered some software updates.

When returning the car, I informed the Sixt representative that I had linked my BMW ID. They assured me the vehicle would be reset. Curious, I checked just before deleting the "My BMW" app — and to my surprise, I still had full remote access:

- Live location tracking  
- Remote lock/unlock  
- Honking (hehe)  
- Turning lights on/off  

By that point, the car was presumably rented out to someone else. I was able to track the new renter’s location and interact with the vehicle remotely.

This situation raises serious security and privacy concerns:
- BMW ConnectedDrive still associated my account with the vehicle's VIN  
- Sixt’s reset procedure did not revoke my BMW ID access  

I suspect this issue isn’t limited to Sixt but could affect other rental fleets using ConnectedDrive if proper backend disassociation isn’t performed. While BMW offers fleet integrations via ConnectedDrive Fleet Services, it’s unclear how many rental cars worldwide still have previous renters’ IDs attached.