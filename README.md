# Personalized Item Recommendation Using T5

### Data Preprocessing:

- Created functions to identify unpurchased items from a list and transform purchase histories.
- Processed data to form recommendation prompts by combining purchased and unpurchased items into structured strings.
- Split data into training and evaluation sets, reformatted as Dataset objects, and built a DatasetDict.
- Tokenized data using a custom preprocessing function with truncation and padding.

### Models and Configuration:

- Used the t5-large model for sequence-to-sequence fine-tuning.
- Set up an optimizer (AdamW) with a linear learning rate scheduler.
- Configured Seq2SeqTrainingArguments with key parameters for batch size, epochs, and weight decay.

### Methodology:

- Used Seq2SeqTrainer to train and evaluate the model.
- Generated predictions, converted tokens back to text, and displayed sample predictions for verification.

### Results:

- Compiled predictions, prompts, and target recommendations into a DataFrame for evaluation.
- Verified the model’s recommendations on sample inputs, achieving expected item recommendations based on the structured prompts
