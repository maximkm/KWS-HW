# KWS-HW
The project is made for educational purposes, as the homework of the course [deep learning for audio processing](https://github.com/markovka17/dla).

## Repository Structure

```bash
checkpoints/                         # The folder where the checkpoints of all trained models are located
models/
├─ kws_baseline_model.pth            # A baseline-based streaming model
├─ kws_final_model.pth               # The final compressed streaming model
main.ipynb                           # A notebook with experiments and a report
stream.py                            # Example of streaming on Windows
stream_mac.py                        # The same streaming, but for Mac
```

## The final score received

| speed up rate | compression rate | streaming |
| ------------- | ------------- | ------------- |
| 10.65 | 10.28 | +  |


## Independent streaming testing

You need to run the code for streaming, it has already configured the loading of the desired model and hyperparameters are configured:
```shell
python stream.py
```

You may have to configure the input device for Windows or Linux, for Mac you can run the script below:
```shell
python stream_mac.py
```
