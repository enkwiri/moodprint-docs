# Data export format

If you choose to export your data from Moodprint, this is what you'll get.

## Example

```json
{
  "moments": [
    {
      "created_at": "2014-08-30T07:25:00Z",
      "notes": "It's a beautiful day",
      "moods": [
        {
          "term": "Content",
          "category": "Joy",
          "intensity": 1
        }, {
          "term": "Hopeful",
          "category": "Optimism",
          "intensity": 2
        }
      ]
    },
    ...
  ]
}
```

## Explanation

When you record your mood with Moodprint, we store it as a **moment**; that's
where we associate the timestamp of the recording, as well as any notes you
provide. Since you can add more than one mood for a single moment, we keep
those as an array of **moods** within the moment; each mood stores the term
that you entered, as well as the category and intensity that have been
associated with that term.
