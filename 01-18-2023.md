# 1/18/2023
# Objectives
- Brainstorm Final Project Ideas
- Work on Initial Post

For this meeting, we initially discussed some ideas that we had in mind prior to taking the class as a group. The first idea was an autonomous robotic wall painter. Some of the details we covered regarding that idea were:
1. The wall painter would use spray paint because a roller would not be very feasible.
2. It would have a color sensor to detect where paint exists on the wall while it maneuvers around it.
3. It would have motors on the chasis for rolling around the wall and would use some sort of suction mechanism.

We discussed the project idea with Professor Gruev after talking amongst ourselves and concluded that it would not be very feasible and would not really necessitate a pcb.

Another idea we discussed was an autonomous leaf raker. This idea would again involve robotics and would be similar
to the wall painter idea. Since this ideas was more realistic we started writing up an initial post for the web board. This is what we came up with:

    PROBLEM: 
    We wanted to incorporate some sort of robotics element and one of the problems we thought of that could use a robot as a solution was raking your leaves. A lot of people who have gardening as a hobby need to clean up their lawns/yards quite often due to leaves falling from trees and ending up all over the place. In a lot of neighborhoods, it is also necessary to keep your yards clean, so automating the process would be quite convenient.

    SOLUTION: 
    Our proposed solution is to create a relatively small robot that pushes the leaves in a lawn/yard to one location for easier cleanup. We are also considering adding a vacuuming element where instead of pushing the leaves to a specific location it just vacuums them into a container and possibly picks up dirt as well. We still need to expand upon this idea and develop it to ensure it is feasible.

    DIFFICULTIES:
    - Determining where leaves are located
    - Mapping the yard/lawn
    - Maneuvering around and over obstacles
    - Ensuring the rake we use doesn't get caught in anything
    - In regard to the vacuuming element we were considering, it would require a lot of storage space and consistently high power.

Our last idea was an autonomous card dealer/shuffler. Again since this idea was more realistic we wrote up an initial web board post:

    CONCEPT:
    We all love card games. To name a few: Poker, Literature, Blackjack, Kings Corner, etc. We all want a fair card distribution system which guarantees the 'dealer' is not cheating.

    USAGE:
    A shuffled deck of cards will be placed in a holder.
    The automatic card dealer may have several modes:

    - distributes cards evenly amongst players for games like Literature and Kings Corner
    - "poker mode" deals flop, turn, river ?
    - "blackjack mode" deals blackjack ?
    - Once the cards have been depleted or the hands have been dealt, the automatic card dealer should ideally stop dealing the cards and enter a sleep mode.

    IMPLEMENTATION:
    As far as actuators/motors, I believe we would need 2. One to control rotation of the trajectory (rotate or move the deck) and one (maybe two) to "pick up the card and throw it".

    As far as sensors, I believe we would need 1 to determine if there are any more cards to deal.

    Let's say there were 3 buttons:
    - Mode,
    - Number of Players
    - On/Off
    - The state machine will always start running to the "next location". When someone presses the button, our machine should stop at the following locations. Assuming +degrees is to the left of the dealer.
        (2player) 0,180, always deal first card to 180 deg position first
        (4player) 0,90,180,270 always deal first card to 90 deg first
        (6player) 0,60,120,180,240,300 always deal first card to 60 deg first
        (8player) 0,45,..., always deal first card to 45 deg first
        Is that something we can do?
