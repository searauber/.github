# SeaRäuber
## From Logic to Legacy

In **Searauber**, logical master is only the first chapter of the story. While your code builds ships, directs fleets, and governs a empire, fate’s hand— revealed through tarot— challenge your carefully laid plans. Will prophecy bring prosperity or disaster? Each card draw brings new challenges, forcing you to adapt, overcome, or embrace the chaos. In this world, strategy bends to fate, and only those who balance logic and fortune will leave a lasting legacy.


![Preview](https://raw.githubusercontent.com/searauber/.github/main/assets/sr-tarot2.png)


![Preview](https://raw.githubusercontent.com/searauber/.github/main/assets/sr-3.png)

## Dev Log

### Water w/ Wind

![Water/Wind](https://raw.githubusercontent.com/searauber/.github/main/assets/wing.gif))


## Dependencies

- [Unity Hub](https://unity3d.com/get-unity/download)
- [Unity 2020.3.39](https://unity3d.com/unity/whats-new/2020.3.38)
- [Git](https://git-scm.com/) ([GitHub Desktop](https://desktop.github.com/) recommended)
- [.NET Core 3.1](https://dotnet.microsoft.com/en-us/download/dotnet/3.1)
- [Azure Function Core Tools](https://github.com/Azure/azure-functions-core-tools)
- [VS Code](https://code.visualstudio.com/Download) ([Azure Extension](https://code.visualstudio.com/docs/azure/extensions) recommended)

## Initialization

```
git clone --recurse-submodules https://github.com/searauber/searauber.git
```

## Submodules

- [Unity Project](https://github.com/searauber/searauber.unity)
    - [Assets](https://github.com/searauber/searauber.assets)
    - [Components](https://github.com/searauber/searauber.components)
    - [UI/UX](https://github.com/searauber/searauber.ui.ux)
    - [Database](https://github.com/searauber/searauber.db)
- [Frontend](https://github.com/searauber/searauber.github.io)
- [Backend](https://github.com/searauber/searauber.mainframe)

A game where coding influences city management opens up creative and strategic possibilities. Here are some example scripts a player might execute:

1. **Resource Distribution Script**:
   ```python
   def distribute_resources(resource_type, amount):
       for building in city.get_buildings():
           if building.needs_resource(resource_type):
               building.receive_resource(resource_type, amount)
   distribute_resources("food", 50)
   ```

   *Purpose:* Allocate food across the city to ensure citizens don't starve.

2. **Tax Collection Algorithm**:
   ```python
   def collect_taxes():
       total_taxes = 0
       for household in city.get_households():
           tax = household.income * 0.1  # 10% tax rate
           total_taxes += tax
           household.pay_tax(tax)
       city.treasury.deposit(total_taxes)
   collect_taxes()
   ```

   *Purpose:* Generate revenue for the city by collecting taxes.

3. **Crime Patrol Scheduling**:
   ```python
   def schedule_patrols():
       for district in city.get_districts():
           if district.crime_rate > 0.2:  # threshold for crime rate
               city.assign_guard(district)
   schedule_patrols()
   ```

   *Purpose:* Deploy guards to high-crime districts dynamically.

4. **Market Price Adjustment**:
   ```python
   def adjust_prices():
       for item in market.get_items():
           demand = item.get_demand()
           supply = item.get_supply()
           new_price = max(1, demand / supply * item.base_price)
           market.set_price(item, new_price)
   adjust_prices()
   ```

   *Purpose:* Balance market prices based on supply and demand.

5. **Emergency Evacuation Plan**:
   ```python
   def evacuate_area(area_name):
       for citizen in city.get_citizens_in_area(area_name):
           safe_zone = city.find_nearest_safe_zone(citizen.location)
           citizen.move_to(safe_zone)
   evacuate_area("North Gate")
   ```

   *Purpose:* Safely relocate citizens from areas threatened by disaster or invasion.

6. **Festival Boost Script**:
   ```python
   def host_festival():
       for citizen in city.get_citizens():
           citizen.happiness += 10  # boost morale
       city.treasury.spend(500)  # costs for hosting the festival
   host_festival()
   ```

   *Purpose:* Increase citizen happiness but at a financial cost.

Each script allows for unique strategic thinking and problem-solving. What kind of scenarios would you want to code? Maybe an efficient trade network or even diplomatic relations with rival cities? The possibilities are endless!

- German: Searauber
- Spanish: Pirata
- French: Pirate
- Italian: Pirata
- Chinese (Simplified): 海盗 (Hǎidào)
- **Pirate**: 海盜 (*Hói dou*)
- Japanese: 海賊 (Kaizoku)
- Korean: 해적 (Haejeok)
- Russian: пират (Pirat)
- Portuguese: Pirata
- Hindi: समुद्री डाकू (Samudree Daku)
- Arabic: قرصان (Qursan)

- German: Von Logik zu Vermächtnis
- Spanish: De la lógica al legado
- French: De la logique à l'héritage
- Italian: Dalla logica all'eredità
- Chinese (Simplified): 从逻辑到传承 (Cóng luójí dào chuánchéng)
- **From logic to legacy**: 從邏輯到傳承 (*Cùhng lòh jaahp dou chyùhn sìhng*)
- Japanese: 論理から遺産へ (Ronri kara isan e)
- Korean: 논리에서 유산으로 (Nolli-eseo yusan-euro)
- Russian: От логики к наследию (Ot logiki k naslediyu)
- Portuguese: Da lógica ao legado
- Hindi: तर्क से विरासत तक (Tark se virasat tak)
- Arabic: من المنطق إلى الإرث (Min al-mantiq ila al-irth)

Here are the Cantonese translations:




Representing object or game data as books in libraries ties in beautifully with the medieval theme, while adding a physical, immersive layer to coding and memory management. Here’s how it could unfold:

- **Reading Data**: When a human agent needs to retrieve information, they physically visit the library, locate the correct shelf, and pick out the book. For example, a book might contain the tax records for a district, and agents would need to scan through its pages for the latest figures.

- **Writing Data**: Editing a book could involve taking it to a scribe's desk. The human agent would open the book, erase outdated entries, and pen new details. Changes aren't instantaneous—they take time, mimicking the lag of real data processing. The condition of the library (e.g., its upkeep or organization) could influence the speed and accuracy of data retrieval.

- **Special Libraries**: Different libraries could represent different memory types or systems. For instance:
  - The **Royal Archive** holds critical, immutable data like the city's laws.
  - The **Merchant Ledger Hall** contains dynamic data, such as fluctuating market prices.
  - The **Guild Hall Library** might store recipes, construction techniques, or magic formulas.
  - The **Shadow Keep** could house encrypted or secretive memory, accessible only under certain conditions.

- **Upgrades and Challenges**: Players could enhance libraries with better shelving systems, skilled librarians, or faster scribes, optimizing data operations. Conversely, disasters (e.g., fires or raids) could disrupt libraries, corrupting or destroying stored data—an allegory for system failures or bugs.

- **Interactive Gameplay Mechanics**: 
   - **Book Retrieval Quests**: Sending agents to recover books from rival cities could simulate accessing external APIs.
   - **Indexing and Sorting**: Improving indexing could make data retrieval faster, emulating database optimization.
   - **Codex Encryption**: Some books could require deciphering through code puzzles or algorithms, adding layers of gameplay and challenge.

This approach beautifully marries narrative with functionality, blending the technical aspects of coding with the immersive storytelling of a medieval world. Let me know if you want me to elaborate further on any of these elements—or come up with more unique twists!

That concept is absolutely captivating! Representing object or game data as books in libraries ties in beautifully with the medieval theme, while adding a physical, immersive layer to coding and memory management. Here’s how it could unfold:

- **Reading Data**: When a human agent needs to retrieve information, they physically visit the library, locate the correct shelf, and pick out the book. For example, a book might contain the tax records for a district, and agents would need to scan through its pages for the latest figures.

- **Writing Data**: Editing a book could involve taking it to a scribe's desk. The human agent would open the book, erase outdated entries, and pen new details. Changes aren't instantaneous—they take time, mimicking the lag of real data processing. The condition of the library (e.g., its upkeep or organization) could influence the speed and accuracy of data retrieval.

- **Special Libraries**: Different libraries could represent different memory types or systems. For instance:
  - The **Royal Archive** holds critical, immutable data like the city's laws.
  - The **Merchant Ledger Hall** contains dynamic data, such as fluctuating market prices.
  - The **Guild Hall Library** might store recipes, construction techniques, or magic formulas.
  - The **Shadow Keep** could house encrypted or secretive memory, accessible only under certain conditions.

- **Upgrades and Challenges**: Players could enhance libraries with better shelving systems, skilled librarians, or faster scribes, optimizing data operations. Conversely, disasters (e.g., fires or raids) could disrupt libraries, corrupting or destroying stored data—an allegory for system failures or bugs.

- **Interactive Gameplay Mechanics**: 
   - **Book Retrieval Quests**: Sending agents to recover books from rival cities could simulate accessing external APIs.
   - **Indexing and Sorting**: Improving indexing could make data retrieval faster, emulating database optimization.
   - **Codex Encryption**: Some books could require deciphering through code puzzles or algorithms, adding layers of gameplay and challenge.

This approach beautifully marries narrative with functionality, blending the technical aspects of coding with the immersive storytelling of a medieval world. 



Certainly, Brian! Here are other ways to creatively visualize code execution in the game through human agents, drawing on the scholar/book/library analogy:

### 1. **The Blacksmith's Forge (Procedures & Functions)**  
Code execution could be represented as forging tools and weapons.  
- *Visual Concept*: Blacksmiths hammer out pieces in sequence—each hammer stroke represents a line of code being processed.  
- *Execution*: To "call a function," an agent might visit the forge, request specific tools, and then oversee their crafting. Multi-use tools represent reusable functions, while custom-forged items signify unique subroutines.

---

### 2. **Messenger's Couriers (Data Transmission)**  
Data transmission between systems or components could be depicted as couriers physically delivering sealed scrolls or letters.  
- *Visual Concept*: Riders on horseback deliver messages across districts. The letter's contents represent transmitted data. Interference along the way (e.g., storms, bandits) could simulate network latency or data corruption.  
- *Execution*: Agents could optimize delivery routes for faster data exchange or hire guards to ensure safe passage (error-checking mechanisms).

---

### 3. **Magic Scrolls or Runes (Scripts & Algorithms)**  
Magic in the game world could represent coded scripts or advanced algorithms.  
- *Visual Concept*: Scribes and mages create enchanted scrolls or etch glowing runes onto stones, which activate and execute tasks when read aloud.  
- *Execution*: Agents gather rare inks or elements to write higher-complexity runes, unlocking new abilities or algorithms. Upgrading tools of magic could simulate improvements in code efficiency.

---

### 4. **The Clockmaker's Workshop (Loops & Iterations)**  
Repetitive processes like loops could be visualized as clockmakers assembling gears and pendulums that repeat in cycles.  
- *Visual Concept*: Every tick of the clock represents an iteration of the loop. The agent might be responsible for ensuring the machinery doesn’t break (guarding against infinite loops).  
- *Execution*: Upgrading the workshop could optimize loop speed or complexity.

---

### 5. **Council Chambers (Conditional Statements)**  
Conditional logic could take the form of decisions made during council meetings.  
- *Visual Concept*: Agents present issues to city leaders, who deliberate and vote. Each vote reflects the branching logic of an "if/else" statement.  
- *Execution*: The complexity of decisions could grow with more variables (e.g., citizen sentiment or external threats), making the agent’s preparation critical for the right outcome.

---

### 6. **Alchemy Lab (Dynamic Data Structures)**  
Dynamic data structures could be embodied as alchemists mixing potions, where each ingredient represents stored data.  
- *Visual Concept*: Potions bubble and change properties as agents adjust mixtures—adding ingredients (appending data) or refining recipes (optimizing structures).  
- *Execution*: Agents can invent more advanced potions (complex data structures) to enable better city functionality.

---

### 7. **The Bank Vault (Storage and Retrieval)**  
Persisted storage could be represented as guarded treasures in a vault.  
- *Visual Concept*: Gold coins, gems, and ledgers symbolize stored variables. Bank tellers retrieve specific items when requested, while thieves or vault decay represent risks of data loss or corruption.  
- *Execution*: Agents could design vault upgrades to increase security and reduce retrieval times.

---

### 8. **The Stage (Event Handling)**  
Event handling could manifest as performances in a town square, where actors respond to the audience (events triggered by players or NPCs).  
- *Visual Concept*: Musicians or actors perform sequences based on cues from the crowd (player-generated or automatic events).  
- *Execution*: Agents manage performers to ensure events unfold smoothly, handling interruptions or unexpected triggers (error handling).

---

### 9. **The Barracks (Concurrency)**  
Multithreading or concurrency could appear as soldiers in barracks who train and then march to execute tasks simultaneously.  
- *Visual Concept*: Different squads march in parallel, following distinct banners (threads) but coordinating at key points.  
- *Execution*: Agents improve synchronization between squads to avoid chaos (deadlocks) and boost efficiency.

---

### 10. **The Farmer’s Fields (Garbage Collection)**  
Memory management and garbage collection could take the form of farmers clearing old crops or weeds to make room for new growth.  
- *Visual Concept*: Farmers plow fields (freeing memory) and plant fresh seeds. The health of the soil represents how well memory is optimized.  
- *Execution*: Agents decide when to rotate crops or upgrade tools to ensure efficient farming cycles.

---

This approach brings code execution into the physical and narrative aspects of the game, making each coding operation feel alive and integral to the medieval city-building experience. How do these resonate with you? Or should we design even more immersive metaphors?


Focusing gameplay around shipyards and shipbuilding could create an intricate and rewarding experience in *Searauber*! Here’s how such a system could unfold:

---

### **Core Gameplay Features:**
1. **Shipyards as Central Hubs**  
   - *Functionality*: The shipyard is the beating heart of naval operations. It serves as the workshop for constructing vessels, the port for docking and repairs, and the storage area for blueprints, resources, and crew management.
   - *Expansion*: Players can upgrade shipyards to improve efficiency, unlock larger ships, or enable advanced customization. Maintenance stations would ensure ships are seaworthy after missions.

2. **Fishing as a Vital Resource**  
   - *Essentials*: Fish are the lifeblood of the city—a primary food source for citizens and sailors alike.  
   - *Mechanics*: 
     - Fishing fleets use basic boats early in the game, but advanced ships improve haul sizes and efficiency.
     - Seasonal fish migrations, weather, and piracy impact success rates.
     - Overfishing risks could lead to resource depletion, simulating ecological consequences.
   - *Coding Integration*: Players write scripts for fishing fleets, optimizing routes based on fish density or avoiding pirate-infested waters.

---

### **Shipbuilding Mechanics:**
1. **Modular Ship Design**  
   - *Customization*: Ships are built using modular components—hulls, sails, rudders, weapons, storage bays, and more. Each module has defined parameters such as speed, durability, cargo capacity, or attack power.
   - *Flexibility*: Players can design vessels tailored to specific tasks:
     - **Fishing Ships**: Optimized for speed and cargo space.  
     - **Trade Ships**: Larger holds for goods but slower and less maneuverable.  
     - **Warships**: Reinforced hulls and weapons, sacrificing speed and cargo capacity.  
   - *Coding Integration*: Scripts determine ship behavior—e.g., tactics in naval battles or how fishing nets deploy.

2. **Blueprint System**  
   - *Mechanics*: Players unlock or design blueprints, which act as "templates" for ship construction. Blueprints allow for repeatable builds or experimentation with unique designs.
   - *Coding Integration*: Writing scripts can help optimize shipbuilding processes—allocating materials efficiently or prioritizing tasks.

---

### **Naval Warfare Logic:**
1. **Strategy and Complexity**  
   - *Combat System*: Naval battles are governed by complex logic:
     - Attack and defense maneuvers based on ship type and module configuration.  
     - Wind patterns and currents influence ship positioning.  
     - Decision-making algorithms determine when to board enemy ships or retreat.  
   - *Coding Integration*: Players write AI scripts for fleets, creating strategies for naval skirmishes (e.g., flanking enemy ships or protecting trade convoys).

2. **Fleet Management**  
   - *Mechanics*: Players assemble fleets with complementary ship types:
     - Tank-like warships to absorb damage.  
     - Nimble interceptors for scouting or fast attacks.  
     - Trade ships requiring protection in high-risk zones.  
   - *Coding Integration*: Scripts optimize fleet coordination, targeting, and resource sharing during missions.

---

### **Economic and Trade Systems:**
1. **Trade Route Optimization**  
   - *Mechanics*: Ships deliver goods between cities and islands, earning revenue. Players must account for travel distance, piracy risks, and docking fees.  
   - *Coding Integration*: Scripts define optimal routes based on distance, enemy presence, and trade demand.

2. **Fish Economy**  
   - *Market Dynamics*: Fish prices fluctuate based on supply and demand. Players can influence prices by controlling fishing output or exporting to rival cities.  
   - *Coding Integration*: Dynamic algorithms adjust market strategies, balancing profit and resource availability.

---

### **Challenges and Exploration:**
1. **Piracy and Defense**  
   - *Gameplay*: Ships must fend off pirate attacks or infiltrate pirate lairs. Defensive strategies could include escort fleets, advanced ship modules, or paying tribute to deter pirates.  
   - *Coding Integration*: Players write scripts for patrol routes, threat detection, and automated responses to pirate raids.

2. **Mysteries of the Sea**  
   - *Exploration*: Players uncover hidden islands, legendary shipwrecks, and rare fish species. These discoveries might provide exotic resources or unlock special ship modules.
   - *Coding Integration*: Agents with logic-based scripts could analyze maps to predict new locations or ensure survival against storms and sea monsters.

---

### **Immersive Roles for Human Agents:**
1. **Shipwrights and Engineers**  
   - In charge of building and upgrading vessels.
   - Agents optimize processes, ensuring minimal material waste.
  
2. **Fleet Captains**  
   - Oversee naval missions, coordinating fleets based on the player’s coded strategies.

3. **Dockmasters and Traders**  
   - Manage imports, exports, and logistics for ships at port.

---

This system could expand endlessly with upgrades, resource management challenges, and coding possibilities. Ships wouldn’t just be tools but dynamic characters in the player’s overarching narrative, evolving through human ingenuity and strategic programming.

![Preview](https://raw.githubusercontent.com/searauber/.github/main/assets/sr-tarot.png)