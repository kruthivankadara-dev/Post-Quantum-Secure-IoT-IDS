Terminal 1 — Cloud Continual Learning Server
python cloud/continual_learning_server.py

Expected:
[CLOUD] Loading CNN-LSTM... ;
[CLOUD] Ready;
Continual Learning Server Started.


Terminal 2 — Edge Gateway
python edge/edge_gateway.py

Expected:
Edge Gateway Started;
Loading CNN-LSTM;
Loading Autoencoder;
Loading Scaler;
Ready.


Terminal 3 — IoT Device Simulator
python iot/device_simulator.py

This simulates multiple IoT devices
Each device:
Establishes a quantum-safe session using ML-KEM
Encrypts telemetry using AES-256-GCM
Sends secure packets to the Edge Gateway
