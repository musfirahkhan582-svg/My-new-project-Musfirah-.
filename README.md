# Musfirah-
Gen ai project 
# GenCabin AI: Nordic Cabin Design & Marketing Generator

Final project for the Building AI course

## Summary

GenCabin AI uses generative AI to design custom Nordic lakeside cabins and auto-generate rental listings. Users input specs like size, sauna area, and lake distance, and the AI outputs floor plans, 3D renders, and SEO-optimized Airbnb descriptions. Building AI course project

## Problems it will solve

* **High design costs**: Custom cabin architecture is expensive and slow. Gen AI cuts concept time from weeks to minutes
* **Poor rental listings**: Many cabin owners lack marketing skills. AI writes compelling, multilingual descriptions that increase bookings
* **Land optimization**: Helps buyers visualize how a cabin fits on a plot given constraints like neighbor distance and lake proximity
* **Personalization at scale**: Lets real estate firms generate unique designs for each client without manual CAD work

## How is it used?

1. **Input parameters**: User enters cabin size (155 m²), sauna size (15 m²), distance to lake (5m), toilets (1), neighbor distance (200m)
2. **AI generation**: Model generates 3 floor plan options + exterior 3D render + interior mood board
3. **Marketing output**: System produces rental listing text, pricing suggestions, and social media posts
4. **Export**: User downloads PDF plans or publishes listing directly to platforms

Example: A landowner with a 5m lakefront plot can see 3 cabin layouts that maximize views while meeting Finnish building codes.

## Data sources and AI methods

**Data sources:**
- 15,000 Nordic cabin floor plans from public architecture archives [ArchDaily](https://www.archdaily.com/)
- Rental performance data from scraped Airbnb listings in Finland, Norway, Sweden
- Satellite imagery for land-use context

**AI methods:**
- **Stable Diffusion + ControlNet**: Generates 3D renders conditioned on floor plan + lake distance
- **GPT-4o fine-tuned**: Writes rental descriptions using high-performing listing data
- **Linear regression**: Predicts rental price based on features like sauna size and lake proximity
- **Genetic algorithm**: Optimizes cabin orientation for privacy given neighbor distance

## Challenges

What does your project _not_ solve? Which limitations remain?

* Does not handle building permits or structural engineering calculations — still requires human architect sign-off
* Limited to rectangular plots; complex terrain not supported yet
* Training data bias: Most cabins in dataset are Finnish, so Norwegian styles may be underrepresented
* AI-generated plans may violate local zoning without manual check

## What next?

How could your project grow and become something real?

1. Partner with My Cabin and other prefab manufacturers to auto-quote builds from AI designs
2. Add VR walkthroughs using NeRF models generated from the floor plans
3. Integrate with municipal GIS APIs to auto-check zoning compliance
4. Expand to other building types: saunas, summer cottages, tiny homes

## Acknowledgments

* University of Helsinki & Reaktor for the Building AI course
* My Cabin prefab data for layout inspiration
* ArchDaily open-source floor plans
* Stable Diffusion community for generative architecture examples
