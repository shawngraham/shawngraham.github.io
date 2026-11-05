# Urbs, Urbis: A Teaching Guide

Nov 4, 2026

Urbs Aeterna is a toy model of an ancient Roman city that you can argue with: every contested claim about how Roman cities worked is a slider, and you watch what the claim does when the city has to feed, house and pacify its people. And of course, you can build the city the way you like.

## Purpose and how to use this guide

The simulation is built for seminars and self-study in Roman social and economic history. It’s not about ‘re-running’ history or re-telling a particular ancient Roman city’s actual history. Instead, it operationalizes various urban and economic theories or systems of explanation using a variety of sliders and settings so you can observe and play with those understandings. It lets you record and compare different systems. (Because it is written in three.js and html, you can open it up with a text editor and find the bits you disagree with, and change things up accordingly if so inclined).

I see this as a complementary strand to exploring ideas about the past, in the same way one might build research-grade agent based models..

How to approach things:

1. Read _The model in brief_ and play _A first session_ (about ten minutes).
2. Skim _The Lex et Mos settings_ and _The readings_ to learn what each slider stands for and who argued it.
3. Work through _Comparing runs_, then try two or three exercises from _Questions raised_.
4. When you disagree with the model, use _Disputing the implementation_ to build your own reading and record the disagreement.

## The model in brief

One turn of the simulation is one month. You lay streets, houses, shops, fountains and monuments on a grid; the city then grows, eats, burns, trades and quarrels according to the rules you set in the Lex et Mos panel.

| Scenario | Start | What you do | Ends when |
| --- | --- | --- | --- |
| Free City | Year 1 AD, a bare river valley | Build as you like, with no goals | You stop |
| --- | --- | --- | --- |
| Colonia (Sullan) | 674 AUC, veterans and a charter | Found a colony and satisfy the Senate's tests | The charter is confirmed, or the colony fails |
| Pompeii | Mid-first century, the city drawn as it stood in AD 79 | Keep water, grain and order; clear ruins; keep gates open | You stop, or Vesuvius erupts (if switched on) |

The top bar shows five numbers.

| Figure | What it measures |
| --- | --- |
| Denarii | The treasury, with the monthly change beside it |
| --- | --- |
| Grain, modii | The public stock, with the monthly change |
| Populus | Free population, with the monthly change |
| Concordia | Public order, 0 to 100. Low order leads to unrest and, at length, to the legions |
| Dignitas | Civic prestige, which rises with temples, the forum, arches and rich houses |

Useful controls: **Space** pauses; the speed buttons run at 1x, 2x or 4x; **T** gives a top-down view; **G** opens the Ledger (the data panel); the **Lens** button colours the ground by water, sewer or service coverage; **Demolish** removes a building; **Inspect** shows what one tile does.

Two things to know before you experiment. First, the city runs from the moment a scenario starts, so press **Space** to pause before you change settings. Second, the model uses chance: fires, price shocks, harvests and the weather differ from run to run, even with identical settings.

## A first session

The Pompeii scenario is the best place to start, because the city is already built and you can watch it behave before you touch anything. Pompeii of course is the city whence many (most?) of our theories of the ancient city emerge.

1. Choose **POMPEII** on the cover page. Press **Space** at once to pause.
2. Open the **Lex** panel on the right and scroll through it without changing anything. Each slider has a one-line summary and a _Why it matters_ link giving a brief synopsis of the scholarly argument behind it.
3. Set the speed to 4x and press **Space** to run. Let two or three years pass. Watch Concordia, the grain figure and the treasury.
4. Press **G** (or the **Data** button). Visit the _People_, _Money_ and _Grain_ tabs. Notice the yearly wave in the grain stock: fields yield most in June to August, and stocks fall through winter.
5. Hover over a chart. The legend shows each series' value at that month.
6. Return to the Ledger's _Events_ tab. Fires, shortages and price shocks are logged there with their dates.
7. Click **Save this run as reference**, and name it "Default rules". The reference remains in your browser after you reload the page.
8. Reload the page, start Pompeii again, and pause. Open Lex and press **About these readings**. Pick one reading, for example _Pompeii: houses and markets_, read its summary and apply it.
9. Run the same number of years. Open the Ledger's _Summary_ tab: it compares this run with the reference at the same month. The charts now show your reference as dashed lines.

What you should now have: a feel for the seasons and the city's rhythms, a reference run, and one comparison. The rest of this guide is about making such comparisons fair, and about reading them.

## The Lex et Mos settings

The Lex panel holds thirty-one sliders in seven groups. Each stands for a disputed claim. The slider's end labels name the two positions; its note names the scholar or source behind them. Sliders interact: moving one rarely changes only one thing.

The tables give each slider's range and default, the claim it represents, and a first experiment. Three groups apply only to some scenarios: _Vesuvius_ appears in Pompeii, _Colonia_ in the Sullan colony, and the rest everywhere else.

The "default" in the tables below is the Sandbox value. The other two scenarios start from their own defaults, and **Reset** and every reading return the unnamed sliders to _that scenario's_ defaults, not to the Free City's.

| Scenario | Defaults that differ from the Sandbox |
| --- | --- |
| Pompeii | Tribute 20, direct tax 0, dole 0, slaves 30, separation 10, storeys 4, fire 70, aqueduct losses 35, games 70, piety 70, producer 60, market form 55, trust 65, elite demand 45, scale 30, immigration 80 |
| --- | --- |
| Colonia | Tribute 35, dole 0, slaves 20 |

### Economy: where the money comes from

| Slider | Range (default) | The claim it stands for | First experiment |
| --- | --- | --- | --- |
| Producer or consumer city | 0 to 100 (35) | Finley's consumer city (low) against cities of real manufacture and exchange (high) | Compare 10 with 90 on treasury and unemployment |
| --- | --- | --- | --- |
| Imperial tribute | 0 to 200% (100) | How much of the budget came from the empire, not the city's own streets | Halve it, then watch which trades fail |
| Direct tax on citizens | 0 to 100% (10) | Italian citizens paid no regular direct tax after the mid-2nd century BC | Raise it: more revenue, more discontent. Where does the break-even lie? |
| Slave labour share | 0 to 80% of jobs (30) | How large the enslaved workforce was, which is argued | Compare 10 with 70 on unemployment and fear |
| Grain price volatility | 0 to 100% (30) | Recurring shortages when harvests or shipping failed | Raise it and watch the price chart and order |
| Harvest variability | 0 to 100% (35) | Garnsey: harvests swung widely from year to year and field to field. At 0 every year is identical | Run 0, 35 and 100 for ten years: compare yields and months of hunger |
| Winter sailing closure | 0 to 100% (50) | The Mediterranean was largely closed to shipping in winter | Set 100 and 0 and compare grain stock in February |

### Bazaar: how markets worked

These four follow Peter Bang's _The Roman Bazaar_ (2008) against more integrated readings of Roman trade.

| Slider | Range (default) | The claim it stands for | First experiment |
| --- | --- | --- | --- |
| Market form | 0 to 100 (40) | Integrated markets (low) against a Geertzian bazaar of scattered buyers and poor price information (high) | At 90, watch how clustering of traders and the trade multiplier move |
| --- | --- | --- | --- |
| Personal ties and brokers | 0 to 100% (50) | Trade ran through trust, patrons and households more than contracts | Place a domus beside shops, then raise it |
| Whose demand drives trade | 0 to 100 (30) | Trade followed the state and the elite who spent tribute (high) or mass demand (low) | Cut tribute at 80, then at 10 |
| Scale of traders | 0 to 100 (50) | Household-scale enterprise (low) against large firms (high) | Compare jobs and returns at 15 and 85 |

### Society: order, belief and neighbours

| Slider | Range (default) | The claim it stands for | First experiment |
| --- | --- | --- | --- |
| Grain dole (cura annonae) | 0 to 100 (20) | Free grain: cheap calm, or a drain on the treasury | Raise it and watch migrants, order and grain revenue |
| --- | --- | --- | --- |
| Patronage (clientela) | 0 to 100 (50) | Poor clients leaned on rich patrons; a domus can calm the insulae around it | Compare 20 with 85 beside a domus |
| Mixed or separated neighbourhoods | 0 to 100 (20) | Wallace-Hadrill found rich and poor on the same streets (low); separation weakens patronage but raises prestige (high) | Compare 0 with 80: elite mood, patronage reach, dignitas |
| Bread and circuses | 0 to 100 (50) | Juvenal's view of spectacle (high) against spectacle as elite display with little political effect (low) | Build an Amphitheatrum, then compare 10 with 90 on order and the cost of shows |
| Weight of civic religion | 0 to 100 (50) | The pax deorum: how far temples calm the crowd and build dignitas | Compare 10 with 90 beside a temple |

### Urban fabric: the physical city

| Slider | Range (default) | The claim it stands for | First experiment |
| --- | --- | --- | --- |
| Insula height limit | 2 to 8 storeys (5) | Tall, rickety tenements, and Augustus's reported cap on height | Compare 3 with 7: capacity against fire and disease |
| --- | --- | --- | --- |
| Fire hazard | 0 to 200% (100) | Fires were chronic; the vigiles answered them | Raise it, then build Vigiles beside the densest blocks |
| Urban graveyard effect | 50 to 200% (100) | Scheidel: ancient cities buried more than they bore and lived on migrants | Raise it and watch whether immigration can keep up |
| Immigration pull | 0 to 200% (100) | Newcomers came for work, grain and spectacle | Halve it and see which cities stagnate |
| Walking range | 50 to 150% (100) | A pedestrian city: how far every service reaches | Shorten it and watch coverage fall on the Services tab |
| Aqueduct losses and theft | 0 to 50% (25) | Frontinus recorded leaks and illegal taps | Raise it and watch the water-supply ratio |

### Urban change: how towns changed use

These three govern the evolution and devolution of buildings. Domus become shops, insulae become tabernae where custom is heavy, and homes are cleared for civic works.

| Slider | Range (default) | The claim it stands for | First experiment |
| --- | --- | --- | --- |
| Land-use fluidity | 0 to 100 (30) | Roman towns changed use as they grew; at 0 every block stays as built | Compare 0 with 80 over twenty years: how many domus survive? |
| --- | --- | --- | --- |
| Elites lease their frontage | 0 to 100 (50) | Wallace-Hadrill: owners rented street rooms as shops | Compare 10 with 85 on shop numbers and elite mood |
| Civic clearance | 0 to 100 (40) | Rulers cleared housing for public works, as Nero and the Flavians did | Designate a theatre site, then watch the pace of buyouts at 10 and 90 |

### Vesuvius (Pompeii only)

| Slider | Range (default) | The claim it stands for | First experiment |
| --- | --- | --- | --- |
| Month of the eruption | January to December (October) | The manuscripts of Pliny give 24 August; an inscription of 2018 and the autumn finds have led some to argue for October | Compare August with October. What changes in the grain stock and the harvest at the time? |
| --- | --- | --- | --- |
| Heed paid to the tremors | 0 to 100% (25) | Seneca: earthquakes in Campania were common and little feared | Compare 0 with 100 on the share of people who get out |

The eruption itself is a separate switch: the checkbox _Vesuvius erupts in AD 79_. No reading changes it, so every comparison is between cities that all face (or all escape) the mountain. This will probably get deleted in a future version, though I think it’s oddly sad to watch the ash cover the city over.

### Colonia (Sullan colony only)

| Slider | Range (default) | The claim it stands for | First experiment |
| --- | --- | --- | --- |
| Veteran loyalty | 0 to 100% (70) | Sulla's veterans owed him land and little else; many drifted to Catiline | Set it low and watch order as veterans remain |
| --- | --- | --- | --- |
| Plot sales | 0 to 100 (40) | Sallust: veterans squandered their grants; richer neighbours bought | Raise it and watch population and farm output |
| Local grievance | 0 to 100 (50) | The old owners lost land; Sullan settlements bred long resentment | Raise it and expect arson and raids |
| Rights for locals | 0 to 100 (20) | At Pompeii the Oscan families were folded into the colony over time | Raise it: less grievance, more settlers, but resentful veterans |

## The readings

A reading is a named set of slider values that stands for various schools of thought re ancient urbanism. Choosing one sets the sliders it names and returns every other slider to the scenario's default (the eruption month and the heed paid to tremors are kept). A reading is therefore a complete rule set: default rules plus the changes below.

The chips at the top of the Lex panel apply readings directly. **About these readings** opens a dialogue with each reading's simulation effect, its historical basis, a caveat, and a table comparing its values with the defaults. Read the caveat before you run: several citations in the game are given from memory and say so.

| Reading | The argument | Sliders it sets | Where |
| --- | --- | --- | --- |
| Reset | Not a position: the baseline from which the others depart | None | Any |
| --- | --- | --- | --- |
| Finley | The consumer city: rents and tribute, marginal trade (_The Ancient Economy_, 1973) | Producer 8, tribute 140, slaves 35, tax 0, dole 30, games 65, price volatility 25, winter closure 70 | Any |
| Hopkins | Taxes drove trade: provincials sold goods to pay coin taxes (JRS, 1980) | Producer 75, tribute 110, tax 25, slaves 25, price volatility 20, winter closure 25, immigration 110 | Any |
| Bang: bazaar | Trade ran through personal networks, tribute and elite demand (_The Roman Bazaar_, 2008) | Market form 85, trust 80, elite demand 75, scale 15, producer 25, tribute 130, price volatility 55 | Any |
| Integrated markets | Prices moved together and trade answered price signals (Temin; Kessler and Temin) | Market form 10, trust 20, elite demand 20, scale 75, producer 70, price volatility 15 | Any |
| Mixed streets | Rich and poor lived on the same streets (Wallace-Hadrill, 1994) | Separation 0, patronage 85, walking 90, storeys 4, piety 55, fluidity 55, leasing 80 | Any |
| Augustus | The princeps tidied the city: height cap, vigiles, temples (Strabo, Dio, Suetonius) | Storeys 4, fire 60, dole 25, games 75, piety 85, immigration 90, tax 5 | Any |
| Graveyard | The city that ate people: deaths exceed births, migrants fill the gap (Scheidel; Morley) | Graveyard 170, immigration 155, storeys 6, leaks 35, fire 130, dole 35 | Any |
| Slave city | Conquest made Italy a slave society (Hopkins, 1978; Bradley, 1994) | Slaves 70, producer 60, dole 15, patronage 70, games 40, tribute 80 | Any |
| Pompeii: houses and markets | Shops built into great houses, with a low-productivity consumer economy (Wallace-Hadrill with Jongman) | Separation 0, patronage 85, walking 90, storeys 3, piety 60, fluidity 60, leasing 85, producer 20, scale 20, elite demand 70, market form 60, trust 75, tribute 20, slaves 30 | Pompeii |
| Hard colonists | A garrison on hostile ground (Sallust; Cicero) | Veteran loyalty 85, grievance 75, local rights 5, plot sales 30, patronage 60 | Colonia |
| Open colony | Folding in the locals (Pompeii, after 80 BC) | Veteran loyalty 55, grievance 25, local rights 80, plot sales 55, immigration 130 | Colonia |

Three habits make readings useful rather than decorative.

- Each reading is an exaggeration for contrast. The Finley reading sets trade low so the contrast is plain, though Finley allowed real trade.
- Notice what a reading leaves alone**.** Hopkins's thesis concerns provincial taxes, yet the game's direct tax falls on citizens, so the setting is only a stand-in. A slider can stand for an argument without capturing it.
- Treat a reading as a hypothesis. Ask what it predicts, run it, and see whether the prediction holds. The model may surprise you; that is the point.

## Comparing runs

The model contains chance, so one run proves little. A comparison is useful only if the two runs differ in the one thing you meant to change, and if that difference is larger than the run-to-run noise. The Ledger helps with the first; you must supply the second.

### The tools

| Tool | What it does | Notes |
| --- | --- | --- |
| Ledger (**G**, or the Data button) | Records dozens of measures every month: people, money by source, order, grain, service coverage, the bazaar multiplier, buildings | Tabs: Summary, People, Money, Order and health, Grain, Services, Bazaar, Buildings, Events |
| --- | --- | --- |
| Hover | Shows each series' value at the month under the cursor | The faint dashed value beside it is the reference run's |
| Markers | Pink dashed lines mark rule changes and readings; small ticks mark events (red bad, amber warning, green good) | Read them before you trust a chart: a mid-run change makes a run a different experiment |
| Reference run | _Save this run as reference_ stores one run. It reappears as dashed lines on every chart, and the Summary tab tabulates the two runs at the same month | One slot only. It survives a page reload in this browser |
| Copy CSV, Save CSV | Exports the current run and the reference: every series, the thirty-one rule values for each month, and the event notes | Save needs a viewer prompt and may be declined; Copy works in most views |

### A fair two-run comparison

1. Start the scenario and press **Space** at once, so nothing happens before your settings are in place.
2. Choose the reading or set the sliders for run A. Note them: name the reference after them (for example "Finley, 10 years").
3. Run a fixed length. Ten years (120 months) is a good minimum; let the early months of start-up settle.
4. Open the Ledger and save the run as the reference.
5. Reload the page and start the same scenario. Pause. Change **one** setting, or apply one other reading.
6. Run the same length. Open the Summary tab.
7. Run both settings again, if you can, and compare the pairs. A difference that reverses between pairs is noise.

### Estimating the noise

Run identical settings twice, save the first as the reference, and look at the Summary for the second. The gaps you see are the noise floor for that measure over that period. Treat any difference between _different_ settings that is smaller than this as unproven.

For a stronger test, collect five runs per setting. Copy the CSV after each into one spreadsheet, keep the _run_ and _scenario_ columns, and take the mean of a measure over the last twelve months of each run. Five means per setting give a rough sense of both the effect and its spread.

### Reading the Summary tab

The table lists population, treasury, order, disease, unemployment, elite mood, dignitas, water supplied, trade multiplier and standing buildings, then counts of months with hunger or epidemic and of fires logged. It compares both runs at the same month and shows the difference. It reports one moment, so scan the charts for the path that led there: two runs can end alike after different journeys.

### Traps

| Trap | Why it misleads | Remedy |
| --- | --- | --- |
| Changing settings mid-run | The run becomes a hybrid; pink markers show where | Set everything at month 0, or deliberately make the change a shock and study the response |
| --- | --- | --- |
| Comparing different layouts | In the Sandbox you build differently each time, which swamps the settings | Compare in Pompeii, where the city is the same, or build identically |
| Judging by a single month | Harvests, fires and prices vary by month and by season | Compare yearly averages, or the same calendar month |
| Ignoring start-up | The first months show the city adjusting from its starting numbers | Skip the first one or two years |
| Reading a small gap as an effect | One run each is a sample of one | Estimate the noise floor, and replicate |
| Forgetting the eruption switch | A city that faces Vesuvius is a different test | Keep _Vesuvius erupts in AD 79_ the same in both runs |

## Things to watch for

The interesting things tend to appear as chains of cause and effect, and as the places where the model disagrees with your expectation. The table lists signals worth checking, where to see them, and what else to look at before you draw a conclusion.

| Signal | Where to look | What it may mean | Check also |
| --- | --- | --- | --- |
| Grain stock falls to zero in late winter | Grain tab; top bar | Harvest too small, sea closed, or storage too small. Hunger follows within a month | Harvest quality chart, winter closure, number of ports and granaries (Horrea) |
| --- | --- | --- | --- |
| Price of grain above about 1.5 | Grain tab | Stocks below a month and a half of cover, or a price shock. Prices above 1.5 add to unrest | Whether a shock (logged as _Annona crisis_) or a shortage caused it |
| Concordia drifts downward | Order and health tab | The stress term is rising or the calming term falling. Order follows its target slowly | Which of hunger, homelessness, unemployment, tax, disease and fear is moving |
| Homeless count rises while capacity is unused | People tab | Housing is in the wrong place, or too few streets reach it | Housing capacity against plebs, street frontage |
| Fire ticks cluster in one district | Events tab; Buildings tab | Tall tenements and no vigiles near them | Insula height limit, fire hazard, Vigiles coverage |
| Disease high and persistent | Order and health tab | Poor water or sewers; crowding; an epidemic month | Services tab: water, sewers, baths; the water supply ratio |
| Shops multiply as houses vanish | Buildings tab; Events | Urban change is converting domus and insulae | Land-use fluidity, leasing, and the shop-demand feedback; elite mood after |
| Trade multiplier stays near 1 | Bazaar tab | Traders are scattered, or no patron reaches them | Market form, trust, elite demand; the clustering line |
| Elite mood falls beside tenements | Order and health tab | Separation is high or elites tolerate neighbours badly | Mixed or separated neighbourhoods; patronage reach |
| People arrive, then leave | People tab | Immigration pull outruns housing or work, or the graveyard effect eats them | Graveyard, immigration, unemployment |

### If this then that...

- **A poor harvest year.** Harvest quality dips; stocks fall; the price rises; hunger or higher prices raise stress; order slips; the legions may be called. Watch how many months each step takes, and whether granaries and ports soften the blow.
- **Clearing a site.** A designated plot is bought out and demolished; displaced crowds add fear; order falls for a while; then the theatre or arena rises and dignitas and calm may recover. Does the exchange pay?
- **Cutting tribute.** Trade depends partly on elite and tribute demand. When tribute falls, shops that depended on elites may fail even though nothing else changed.
- **Taller tenements.** More people fit in the same ground, but fire spreads further and disease finds crowds. Look for the height at which the city starts to lose more than it gains.

### Things the model does by design that you may mistake for results

- Every month is one step. Anything that happens faster or slower than a month is rounded to it.
- Seasons come from a fixed harvest curve (low in winter, high from June to August) and a fixed shipping calendar. The yearly variation in quality, timing and fleets is random and set by the _Harvest variability_ slider.
- Storage is limited: the granary cap applies after each month's eating, so a harvest glut beyond the cap is lost.
- Starting figures are not measured. The first year of any run shows the city settling.
- Fire, plague, price shocks and mobs are random events. A single run may have none of them.
- The Pompeii map is a fixed plan of the city as it was in AD 79, set at 70 BC. Its buildings change through the urban-change rules, and by what you build.

## Questions raised

The questions below grow from the model's structure. Some can be answered by running it, though the answer will always be "in this model". Others are about the model itself and are better argued in seminar.

### Questions the model can help you explore

- **Fed by whom?** In a city that eats from its own fields and from imports, how much storage and shipping does it take to survive a run of bad harvests? Does a dole help or hurt in the worst years?
- **Did spectacle buy order?** How much calm does an arena buy per denarius at _Bread and circuses_ 10 and at 90? When does the same money do more in a temple, a bath or a granary?
- **Does height pay?** At what storey limit do the gains in housing stop covering the costs in fire and disease?
- **Do mixed streets help?** Is a city of mixed neighbourhoods more orderly than a separated one, and does the answer depend on whether patronage binds?
- **What does a bazaar need?** Under a Bang reading, why do traders cluster, and what happens to the poor far from a market when bread is dear?
- **Can a city live on tribute?** If tribute falls by half, which trades fail first, and does the Hopkins reading survive the cut better than the Finley one?
- **Who pays for the Flavian arena?** How do buyouts, clearance and displaced crowds change the cost of a monument, and does the Civic clearance rule shift who bears it?

### Questions about the model itself

- **Is a slider the right unit?** A claim such as "trade was marginal" has several parts. Does one slider capture it, or merely one consequence?
- **What is missing?** The model has no credit, no law courts, no festival calendar and no countryside beyond the fields. Which absence matters most for the argument you are testing?
- **Are the defaults neutral?** The baseline is a middle reading. Is there any neutral position, or does every default carry a thesis?
- **What counts as success?** The model scores a city by order, population, dignitas and the treasury. Whose measure of a good city is that? What would a Roman writer have valued?
- **What can a toy teach?** If the model reproduces a pattern you expected, has it confirmed anything? If it does not, who should be doubted first?

### Five exercises

| Exercise | Setup | Record | Discuss |
| --- | --- | --- | --- |
| 1\. The weather | Pompeii, default rules. Harvest variability at 0, 35 and 100, three runs each, ten years | Yearly grain grown; months of hunger; lowest Concordia | How much storage would have protected the city at 100? |
| --- | --- | --- | --- |
| 2\. Finley against Hopkins | Pompeii, readings Finley and Hopkins, ten years each, two runs each | Treasury, unemployment, trade multiplier, order | Which results follow from the sliders alone, and which surprise you? |
| 3\. Streets and fire | Pompeii, _Mixed streets_ against _Augustus_, fifteen years, three runs each | Fires logged, standing buildings, disease | Did the cap on height or the mix of neighbours matter more? |
| 4\. A theatre site | Pompeii, designate a Theatrum site beside a street at clearance 10 and 90 | Months to clear; fear; order; treasury | Does faster clearance help the city, or only the monument? |
| 5\. The warning | Pompeii with the eruption on, heed at 0 and at 100, October | Share who escaped; gates open | Which of the two mattered more, and why might a Roman not have known? |

For each exercise, write a one-paragraph hypothesis before the run, and a short note afterwards on what you got wrong.

## Disputing the implementation

You will disagree with some of what the model does. That is useful: a disagreement that can be stated precisely is a research question. The sliders exist so that you can state it in the model's own terms.

### Three kinds of dispute

| Kind | Example | What you can do |
| --- | --- | --- |
| **Value**: you would set a slider differently | "Pompeii's slave share was nearer 15 than 30" | Build your own reading (below) and run it |
| --- | --- | --- |
| **Mapping**: the slider does not represent the claim | "Hopkins's argument is about provincial taxes, but the tax slider hits citizens" | Pick the nearest slider, say so, and note what it leaves out |
| **Structure**: a mechanism is missing or wrong | "Order should depend on food prices in the neighbourhood, not the city" | Sliders cannot change this. Record the objection and its evidence; it needs a change to the program |

### Which slider answers which dispute

| If you dispute | Start with |
| --- | --- |
| Whether the city lived on tribute or on its own production | Producer or consumer; tribute; scale of traders; elite demand |
| --- | --- |
| How markets worked | Market form; trust; scale of traders; elite demand |
| How secure the food supply was | Harvest variability; price volatility; winter closure; grain dole; storeys of granaries you build |
| Whether the rich and the poor were segregated | Mixed or separated; patronage; leasing of frontage |
| How dangerous the city was to live in | Graveyard effect; immigration; fire hazard; storeys; aqueduct losses |
| How much towns changed use | Land-use fluidity; leasing; civic clearance |
| How large and how restless the enslaved workforce was | Slave labour share; patronage; games |
| How far religion and spectacle kept order | Piety; bread and circuses; patronage |

### Building your own reading

1. **Start from the nearest reading.** Apply it, so that you begin from a coherent set of values and not from scratch.
2. **Change the sliders you dispute.** Move one at a time, and write down why. Moving several at once makes it impossible to say which did what.
3. **Watch the Ledger's label.** It marks a reading you have altered with an asterisk, and a pink line marks each change. Your altered reading is now a new, unnamed reading.
4. **Record the values.** The game does not save a custom reading, and it is gone when you reload the page. Write the values down, or copy them from the CSV: every export carries all thirty-one slider values for every month, in columns named _rule\__ followed by the slider's short name.
5. **Name the reference run after your reading** (for example "My Pompeii, horrea 15"), so that a later run is compared with something you can identify.
6. **State the prediction before you run**, and the result after. If the model contradicts you, say so and decide whether to doubt the model, the setting or your own claim.

A record sheet is useful for every reading you build. Paste this into a spreadsheet; the first row names the sliders in the order they appear in the CSV, and the second is for your values.

reading,prod,tribute,tax,slave,vol,hvar,winter,bazaar,trust,eliteDem,scale,dole,patron,seg,games,piety,storeys,fire,grave,immig,walk,leak,fluid,lease,clear,vdate,vheed,vloyal,landsale,resent,cit
my reading,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,

You can read each scenario's default off the _Reset_ reading in **About these readings**, or off the Lex panel before you change anything.

### What the sliders cannot change

Some features are structural. They are the model's own assumptions, and a slider cannot move them.

- Time runs in whole months, on a grid of forty-four by forty-four tiles.
- The population has two free classes, plebs and elites, with the enslaved estimated from the slave-labour share.
- Public order is one number for the whole city, formed from a stress term and a calming term.
- Grain is one commodity with one citywide price. The seasonal curve of harvests and the shipping calendar are fixed in shape, and only their size, timing and luck vary.
- Services reach out to a set distance and weaken with it.
- The rules for converting, clearing and rebuilding buildings, and the monuments' effects on prestige, are chosen by the model's author. They are plausible stand-ins, not measurements.
- Starting stocks, building costs and the sizes of events are not calibrated to any dataset.

### Recording a disagreement

When the sliders cannot express your objection, write it down in a form that someone could act on. Open up the source code. See what might be changed.

| Item | What to put |
| --- | --- |
| The claim in the model | Which behaviour you object to, in one sentence |
| --- | --- |
| Where you saw it | The scenario, reading, month and the Ledger tab |
| Your evidence | The source and what it says (a page or inscription, not a recollection) |
| What you expect instead | The direction and rough size of the effect |
| The nearest slider workaround | What you set, and what it still gets wrong |
| Run files | The CSV of your run and of the reference |

## Things to remember

This is just a toy, and it forces every historiographic claim into a number.

- **It is not evidence.** A result shows what follows from a set of assumptions. It does not show what happened in Pompeii or Rome.
- **It is not calibrated.** Costs, rates, starting stocks and the sizes of effects are set to give plausible behaviour, not fitted to data. The model's author chose the conversion, clearance and prestige rules.
- **Chance is part of it.** Fires, price shocks, harvests and mobs are random. A single run is a story, not a result.
- **It abstracts people.** The enslaved appear as a share of jobs and a risk of revolt; the dead of Vesuvius appear as a percentage. All digital tools involve some kind of abstraction. It’s worth considering what gets abstracted, how, and for what end.
