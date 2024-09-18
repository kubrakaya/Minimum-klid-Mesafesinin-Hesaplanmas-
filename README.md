# Minimum Öklid Mesafesinin Hesaplanması
import math

def euclideanDistance(point1, point2):
    return math.sqrt((point1[0] - point2[0])**2 + (point1[1] - point2[1])**2)

points = [(1, 2), (3, 4), (5, 6)]

distances = []

for i in range(len(points)):
    for j in range(i+1, len(points)):
        distance = euclideanDistance(points[i], points[j])
        distances.append(distance)

min_distance = min(distances)

print(distances)
print(min_distance)
