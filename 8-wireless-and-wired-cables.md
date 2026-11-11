Wired and Wireless Networking: Study Notes

Networking basics, media and cables. Read top to bottom.

Definitions

Wired networking: devices are connected by a physical medium, usually copper wire or glass fibre. Data travels as electrical signals in copper, or as light pulses in fibre.

Wireless networking: data moves through air using radio waves, infrared or light. There is no physical cable between your device and the access point.

Watch out: people say “wireless cable” all the time, but there isn’t one. Wireless only means no cable between the device and the access point. That access point is still usually wired to the internet, so most home setups use both.

Table of Contents

- Wired media

- Twisted pair (UTP, STP) and RJ45

- Coaxial cable

- Fibre optic cable

- Wireless media

- Wi-Fi

- Bluetooth

- Cellular (4G and 5G)

- Satellite

- Infrared

- Mind map

- Flowchart: choosing a medium

Part 1: Wired media

Wired is the older and more predictable choice. It is usually faster and more secure than wireless, but someone has to physically run the cable, so placement is fixed.

1. Twisted pair cable (UTP and STP)

Eight thin copper wires arranged as four pairs, and each pair is twisted. The twists cancel out the electrical noise that neighbouring pairs would otherwise cause (crosstalk). This is the cable behind most office and home network points, with an RJ45 plug on each end.

UTP cross-section: four twisted pairs inside one jacket

Types: UTP (unshielded) is cheap and the most common. STP (shielded) has foil or braid around the pairs, which helps where there is a lot of interference, like factories.

Categories: Cat5e does 1 Gbps up to 100 m. Cat6 does 1 Gbps at 100 m and 10 Gbps over shorter runs. Cat6a does 10 Gbps at 100 m. Cat8 reaches 25 to 40 Gbps but only about 30 m, so it is mostly used inside data centres.

Real-world use: connecting a PC or printer to a switch, and powering IP cameras or Wi-Fi access points through PoE (Power over Ethernet).

Example: the Cat6 cable running from a classroom wall socket to the switch in the server room.

Advantages: cheap, easy to install and fix, PoE can power devices, speed is stable and predictable.
 Disadvantages: has to be routed through walls and ceilings, can’t be used on the move, sharp bends and kinks damage it.
 Limitations: one Ethernet run is capped at 100 m, and your real speed depends on the category you bought.

Straight-through or crossover (exam favourite): a straight-through cable uses the same wiring standard (usually T568B) at both ends and joins unlike devices, like a PC and a switch. A crossover cable swaps the transmit and receive pairs and was used to join similar devices, like PC to PC. Most modern gear has auto-MDI-X, so either cable usually works now.

Memory trick: unlike devices, straight. Like devices, cross.

2. Coaxial cable

One copper core in the centre, wrapped in plastic insulation, then a metal shield, then the outer jacket. The shield blocks outside noise, so coax carries signals further and cleaner than the old unshielded copper pairs.

Coax cross-section: core, insulation, braided shield, jacket

Types: RG-59 is thin and used for short CCTV runs. RG-6 is thicker with lower loss, and it is what cable TV and cable broadband use. Thin and thick Ethernet (10BASE2 and 10BASE5) also used coax, but they are obsolete now.

Real-world use: cable TV, cable internet modems, CCTV cameras, and the lead from a satellite dish to its receiver.

Example: the coax from the wall socket into your cable modem.

Advantages: good shielding, one line can carry TV and internet together, sturdy outdoors.
 Disadvantages: thick and stiff to route, connectors need careful crimping, signal weakens over long runs.
 Limitations: cable internet bandwidth is shared by everyone on the same neighbourhood node, and coax isn’t used for new office LANs any more.

3. Fibre optic cable

Data goes as pulses of light down a thin glass core. The cladding around the core has a lower refractive index, so light keeps bouncing back in by total internal reflection instead of escaping. A plastic jacket protects the whole thing.

Fibre cross-section: glass core and cladding inside a jacket

Types: single-mode (SMF) has a very thin core and one light path. It uses lasers and covers many kilometres. Multimode (MMF) has a wider core with many light paths, uses cheaper LEDs, and suits runs of a few hundred metres. Common connectors are LC, SC and ST.

Real-world use: ISP backbones, undersea cables, links between data centres, and fibre-to-the-home (FTTH).

Example: the fibre from the street cabinet into your house, ending in a small box called an ONT.

Advantages: huge bandwidth, very long distances, immune to electrical interference, very hard to tap without being noticed.
 Disadvantages: expensive to install, glass breaks at tight bends, needs special tools like a fusion splicer and trained staff.
 Limitations: carries no electrical power, so devices need their own supply, and repairs take longer than swapping copper.

Part 2: Wireless media

Wireless is all about freedom of movement. The trade-off is that the air is shared and noisy, so speed, range and security need more care.

4. Wi-Fi (IEEE 802.11)

Wi-Fi uses radio in unlicensed bands: 2.4 GHz, 5 GHz and 6 GHz. Your device joins an access point (usually the home router), and the router is wired to the internet. This is called infrastructure mode. In ad hoc mode two devices talk directly, with no access point.

Standards to remember: 802.11n is Wi-Fi 4, 802.11ac is Wi-Fi 5, 802.11ax is Wi-Fi 6 (6E when it uses the 6 GHz band), and 802.11be is Wi-Fi 7.

[Figure: Router / Laptop / Phone]

Home Wi-Fi: the router sends signal to every device in range

Real-world use: home internet, offices, cafés, airports and smart-home gadgets.

Example: a laptop joins the 5 GHz band of the home router for fast downloads, while an old smart plug stays on 2.4 GHz because it only supports that band.

Advantages: mobility, no drilling or cabling, quick to set up, many devices at once.
 Disadvantages: slower and less stable than wired, weakened by walls, risky if you use WEP or an open network.
 Limitations: indoor range is usually tens of metres. 2.4 GHz has only about three channels that don’t overlap (1, 6 and 11 are the usual picks), so it gets crowded. All devices share the same airtime, so each one slows down as more join.

5. Bluetooth

A short-range radio standard for personal area networks (PANs). Devices have to pair before they talk, and the usual range is about 10 metres. Bluetooth Low Energy (BLE) is a lighter version for sensors and trackers that run on small batteries.

[Figure: Phone / Bluetooth, about 10 m]

Phone to earbuds over Bluetooth

Real-world use: wireless earbuds, keyboards and mice, car audio, fitness bands and smart locks.

Example: your phone sending music to a pair of earbuds in your pocket.

Advantages: very low power, cheap chips, easy pairing, needs no router or access point.
 Disadvantages: short range, slow for anything large, pairing can be fiddly.
 Limitations: it shares the 2.4 GHz band with Wi-Fi and microwave ovens, so interference happens. It is not meant to cover a whole house.

6. Cellular (4G LTE and 5G)

Mobile operators run this on licensed spectrum. Your phone connects to the nearest base station (the tower), and towers link into the operator’s core network. When you move, the connection is handed over from one tower to the next. 5G uses low, mid and high (mmWave) bands. mmWave is very fast but only reaches a short distance.

[Figure: Base station]

Your phone connects to the nearest base station

Real-world use: smartphones, mobile broadband, SIM-based trackers and smart meters, and a backup link when the fixed line fails.

Example: a 4G dongle giving a laptop internet in a village where fibre hasn’t reached yet.

Advantages: wide coverage, works while moving, no cable needed for each user.
 Disadvantages: data plans and caps, weak signal inside thick buildings, higher latency than wired.
 Limitations: speed depends on your distance from the tower and how many people share that cell. Spectrum licences are expensive, so some areas stay under-served.

7. Satellite

A ground dish sends a signal up to a satellite, which beams it back down to another ground station or user terminal. Orbit height matters a lot. GEO satellites sit about 35,786 km up and look fixed from one spot, but the delay is roughly half a second. LEO satellites fly several hundred km up, so latency is much lower, but you need a large group of them for constant coverage.

[Figure: Satellite]

The signal goes up to the satellite and back down

Real-world use: remote villages, ships, aircraft, disaster relief and rural broadband.

Example: a LEO dish fixed on the roof of a house in a hill village, where laying cable would cost too much.

Advantages: works almost anywhere with a clear view of the sky, and no ground cable is needed.
 Disadvantages: higher cost, heavy rain can weaken the signal (rain fade), and it needs a clear view of the sky.
 Limitations: capacity is limited and shared, and LEO coverage depends on how many satellites are in orbit.

8. Infrared

Infrared is light just beyond visible red. It needs a clear line of sight between sender and receiver. TV remotes use it, and older short-range data links (IrDA) did too.

[Figure: Remote / TV]

The remote has to point at the TV with nothing in the way

Real-world use: TV and air-conditioner remotes, some motion sensors, and older short point-to-point links.

Example: pressing volume up on the remote, and the TV’s sensor reading the coded pulse.

Advantages: cheap, low power, the signal stays in the room because walls block it, and it causes no radio interference.
 Disadvantages: needs line of sight, very short range, slow, and strong sunlight can drown the signal out.
 Limitations: not used for general networking now, since Wi-Fi and Bluetooth do the job better.

Mind map

Use this to revise the whole topic at a glance.

[Figure: Networking media / Wired / Wireless / Twisted pair / Coaxial / Fibre optic / Wi-Fi / Bluetooth / Cellular (4G/5G) / Satellite / Infrared]

Mind map: wired and wireless media and their types

Flowchart: choosing a medium

Start at the top and follow the answers. Diamonds are questions.

[Figure: Need to connect a device / Is the device / stationary? / Yes / Over 100 m or / huge speed? / Yes / No / Fibre optic / Twisted pair (Cat6) / No / Wide-area / coverage? / Yes / Cellular or / satellite / No / Under ~10 m? / Yes / Bluetooth or IR / No / Wi-Fi]

Flowchart for picking a medium

In words: if the device is fixed and needs long distance or very high speed, use fibre. If it is fixed and nearby, use twisted pair. If it moves across a wide area, use cellular or satellite. If it moves and only needs a few metres, use Bluetooth or infrared. Anything else that moves around a building or campus goes on Wi-Fi.