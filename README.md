### Functionality Table
```
from seedguard import seedpipe

learner = seedpipe.Learner()    # Create Learner instance to access model related functionalites
evaluator = seedpipe.Evaluator() # Create Evaluator instance to evaluate the model performance and poison attack quality
```
| Usage                               | Functionality                                 | Input                                      | Output                     |
|-------------------------------------|-----------------------------------------------|--------------------------------------------|----------------------------|
| learner.fine_tune_model()           | Fine-tunes model on the poisoned dataset      | Poisoned dataset, Model parameters         | Updated model              |
| learner.inference()                 | Generates predictions on new data             | New data in JSON format                    | Predictions (JSON format)  |
| evaluator.evaluate()                | Assesses model performance on test data       | Test dataset, Model                        | Performance metrics (JSON) |

