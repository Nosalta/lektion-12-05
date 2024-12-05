# lektion-12-05
Lesson on the 5th of December with Niklas

## API:er 
- När det kommer till API:Er och när man gör en Fetch-förfrågan så måste dess options, så är GET standard, och dem vanligaste är ju GET; POST; PUT och DELETE: Om man inte skriver någonting, så är det per automatik GET som körs

``` 
const options = {
  method: "POST",
};
```

 - Låter dig skicka extra information, såsom vilken typ av data du skickar (t.ex. JSON).

Vanligt att specificera Content-Type när du skickar JSON-data.

```
const options = {
  headers: {
    "Content-Type": "application/json",
  },
};
```

- body: Innehåller data som du skickar till servern. Vanligtvis JSON-strängar.

Används endast med metoder som skickar data (som POST och PUT).
´´´
const options = {
  method: "POST",
  headers: {
    "Content-Type": "application/json",
  },
  body: JSON.stringify({
    name: "John Doe",
    email: "john.doe@example.com",
  }),
};
´´´




