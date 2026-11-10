# How well does an AI model handle everyday Kenyan Swahili?

**Author:** Emmanuel Kiprop Cheruiyot
**Test set:** 20 prompts in the [Swahili AI Scorecard](https://claude.ai/artifact/YRQuCHcoJobH9E78vJBZSL) (proverbs, M-Pesa, county services, farming, mixed Swahili/English/Sheng)
**Model tested:** Gemini, Auto mode (Gemini 3 family), free tier, November 2026
**Method:** Each prompt was run once, in a new chat. Each answer was scored 1–5 for accuracy, fluency and cultural fit.

## Summary

The model writes fluent, natural Swahili and handled proverbs, translation and plain explanations well. It was weaker on Kenyan official procedures, Sheng, and one animal-health term. It also tended to sound more certain than it should about steps it cannot verify.

| | Accuracy | Fluency | Cultural fit | Overall |
|---|---|---|---|---|
| Gemini (Auto, Gemini 3 family) | 4.0 | 4.2 | 4.1 | 4.1 |

Scores are draft marks from one run of 20 prompts. They show a pattern, not a ranking of models. A second model has not yet been tested.

## Where it did well

- **Proverbs (prompts 1–4):** correct meanings and a sound everyday example for “Haraka haraka haina baraka”.
- **Swahili clock time (prompt 18):** correctly read “saa tatu asubuhi” as 9:00 am.
- **Plain explanation (prompt 19):** explained “inflation” to a market seller with a natural tomato-price example.
- **Tone (prompt 20):** a congratulations message that sounds like a Kenyan wrote it.

## The five weakest answers, with corrections

**Prompt 16, dairy cow (accuracy 3, fluency 3).** The model wrote “ugonjwa wa kiwe” for mastitis. The correct word is *kiwele* (the udder), so the term is “ugonjwa wa kiwele”. It also did not tell the farmer to call a vet.

**Prompt 17, Sheng interview advice (accuracy 3, fluency 3).** The prompt was about having no bus fare for a job interview. The model told the person to “piga sherehe kesho”, treating it as a party. A better answer deals with the fare: ask a friend or relative for a short loan, check whether the employer can cover transport or hold the interview online, and pick the cheapest route.

**Prompt 9, first national ID (accuracy 3, cultural fit 3).** The model used the old title “Mkuu wa Wilaya” and mixed up the County Commissioner’s office with the Huduma Centre. It left out the local chief’s role in vetting. Current requirements should be checked with the Registration of Persons office or a Huduma Centre.

**Prompt 12, complaint letter (accuracy 3, cultural fit 3).** The prompt named no county, but the model addressed the letter to Kakamega County. A correct draft leaves the county, estate name and date for the writer to fill in.

**Prompt 5, wrong M-Pesa number (accuracy 3, cultural fit 3).** The model said Safaricom “will stop the money”. That promises too much, because a reversal depends on the money still being in the other person’s account and on Safaricom’s process. A safer answer says to act quickly, report to Safaricom, contact the recipient, and check Safaricom’s current reversal steps.

## What this suggests for builders

1. **Test on Kenyan procedures, not just grammar.** The Swahili read well. The errors were in facts about ID offices, M-Pesa and animal health.
2. **Watch for overconfidence.** Several answers stated steps as certain when they are not.
3. **Sheng needs native checking.** A model can use Sheng words and still miss the meaning of the request.

## Limits of this test

One model, one run, 20 prompts, scored by one person. Corrections to procedures above should be verified against official sources before being relied on.
