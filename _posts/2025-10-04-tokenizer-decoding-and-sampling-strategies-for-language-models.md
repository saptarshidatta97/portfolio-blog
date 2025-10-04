---
title: Tokenizer Decoding and Sampling Strategies for Language Models
---


tokenization is the process in the NLP pipeline where 

```Python3
output_ids = model.generate(input_ids, max_new_tokens=20)
decoded_text = tokenizer.decode(output_ids[0])

print("Input IDs", input_ids[0])
print("Output IDs", output_ids)
print(f"Generated text: {decoded_text}")
```
