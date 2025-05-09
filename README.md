# env-code-example:
This repository will contain code examples related to environmental data processing and analysis.
# Content from Assignment 2 solutions
def calculate_average(values):
    if len(values) == 0:
        return 0
    return sum(values) / len(values)

stations = [
    ['A1', 62],
    ['B5', 97],
    ['C3', 155]
]

def report_status(stations, threshold):
    for station in stations:
        id, pm25 = station
        status = "safe" if pm25 < threshold else "danger!"
        print(f"{id} → {pm25} µg/m³ ({status})")
