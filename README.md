# Merge crew

## Plan
Compare models performance on scand eval and create the best model automatically.

## Parameters to check

Model	Configuration
https://huggingface.co/RJuro/munin-neuralbeagle-7b	"models:
  - model: danish-foundation-models/munin-7b-alpha
    # No parameters necessary for base model
  - model: mlabonne/NeuralBeagle14-7B
    parameters:
      density: 0.53
      weight: 0.6
merge_method: dare_ties
base_model: danish-foundation-models/munin-7b-alpha
parameters:
  int8_mask: true
dtype: bfloat16"
very high	"models:
  - model: danish-foundation-models/munin-7b-alpha
    # No parameters necessary for base model
  - model: mlabonne/NeuralBeagle14-7B
    parameters:
      density: 0.9
      weight: 0.6
merge_method: dare_ties
base_model: danish-foundation-models/munin-7b-alpha
parameters:
  int8_mask: true
dtype: bfloat16"
high	"models:
  - model: danish-foundation-models/munin-7b-alpha
    # No parameters necessary for base model
  - model: mlabonne/NeuralBeagle14-7B
    parameters:
      density: 0.7
      weight: 0.6
merge_method: dare_ties
base_model: danish-foundation-models/munin-7b-alpha
parameters:
  int8_mask: true
dtype: bfloat16"
low	"models:
  - model: danish-foundation-models/munin-7b-alpha
    # No parameters necessary for base model
  - model: mlabonne/NeuralBeagle14-7B
    parameters:
      density: 0.3
      weight: 0.6
merge_method: dare_ties
base_model: danish-foundation-models/munin-7b-alpha
parameters:
  int8_mask: true
dtype: bfloat16"
very low	"models:
  - model: danish-foundation-models/munin-7b-alpha
    # No parameters necessary for base model
  - model: mlabonne/NeuralBeagle14-7B
    parameters:
      density: 0.1
      weight: 0.6
merge_method: dare_ties
base_model: danish-foundation-models/munin-7b-alpha
parameters:
  int8_mask: true
dtype: bfloat16"
