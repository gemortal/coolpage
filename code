import time
import math

start_time = time.time()

print("Tracking time drift. Press Ctrl+C to stop.\n")

try:
    while True:
        now = time.time()
        elapsed = now - start_time

        integer_time = int(elapsed)
        fractional_time = elapsed - integer_time

        drift = math.sin(elapsed) * fractional_time

        print(
            f"t = {integer_time}s | "
            f"fraction = {fractional_time:.6f} | "
            f"drift = {drift:.6f}"
        )

        time.sleep(0.5)

except KeyboardInterrupt:
    print("\nStopped. Time keeps going anyway")