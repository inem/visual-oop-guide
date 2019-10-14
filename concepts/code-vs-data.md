code: 

```
  def normalize_letter(letter)
    return "И" if letter == "Й"
    return "Е" if letter == "Ё"
    return letter
  end
```

data:

```
  def normalize_letter(letter)
    identicals = {
      "Й" => "И",
      "Ё" => "Е",
    }
    
    identicals.fetch(letter, letter)
  end
```
