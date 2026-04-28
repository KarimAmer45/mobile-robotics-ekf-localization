# EKF Localization

Extended Kalman Filter localization with odometry prediction and range-bearing landmark corrections. The code also simulates sensor failures and frequency mismatch between odometry and landmark observations.

## Run

```bash
python - <<'PY'
import ex5

mu, covariance, last_control = ex5.run_ekf_localization(plot=False, step_size=100, last_step=400)
print("mu:", mu)
print("covariance diagonal:", covariance.diagonal())
PY
```
