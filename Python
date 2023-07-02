def calculate_apache_ii_score():
    # Step 1: Gather patient information
    age = int(input("Enter patient's age: "))
    temperature = float(input("Enter patient's temperature (in Celsius): "))
    mean_bp = float(input("Enter patient's mean arterial blood pressure: "))
    heart_rate = int(input("Enter patient's heart rate: "))
    respiratory_rate = int(input("Enter patient's respiratory rate: "))
    ph = float(input("Enter patient's arterial pH: "))
    sodium = int(input("Enter patient's serum sodium level: "))
    potassium = float(input("Enter patient's serum potassium level: "))
    creatinine = float(input("Enter patient's serum creatinine level: "))
    hematocrit = float(input("Enter patient's hematocrit level: "))
    wbc = float(input("Enter patient's white blood cell count: "))
    glasgow_coma_scale = int(input("Enter patient's Glasgow Coma Scale score: "))

    # Step 2: Calculate the APACHE II score
    apache_score = 0
    
    # Age points
    if age >= 70:
        apache_score += 3
    elif age >= 55:
        apache_score += 2
    elif age >= 40:
        apache_score += 1

    # Temperature points
    if temperature < 35 or temperature > 39:
        apache_score += 3
    elif temperature <= 34 or temperature >= 38:
        apache_score += 1

    # Mean arterial blood pressure points
    if mean_bp < 70:
        apache_score += 2
    elif mean_bp < 50:
        apache_score += 3

    # Heart rate points
    if heart_rate >= 180:
        apache_score += 4
    elif heart_rate >= 140:
        apache_score += 3
    elif heart_rate >= 110:
        apache_score += 2
    elif heart_rate >= 70:
        apache_score += 1

    # Respiratory rate points
    if respiratory_rate >= 50:
        apache_score += 4
    elif respiratory_rate >= 35:
        apache_score += 3
    elif respiratory_rate >= 25:
        apache_score += 1

    # Arterial pH points
    if ph < 7.15:
        apache_score += 4
    elif ph < 7.25:
        apache_score += 3
    elif ph < 7.33:
        apache_score += 1

    # Serum sodium points
    if sodium < 120:
        apache_score += 4
    elif sodium < 130:
        apache_score += 3
    elif sodium < 150:
        apache_score += 1

    # Serum potassium points
    if potassium > 6:
        apache_score += 3
    elif potassium >= 5.5:
        apache_score += 2
    elif potassium >= 3.5:
        apache_score += 1

    # Serum creatinine points
    if creatinine > 3.5:
        apache_score += 2
    elif creatinine >= 2:
        apache_score += 1

    # Hematocrit points
    if hematocrit < 20:
        apache_score += 4
    elif hematocrit < 30:
        apache_score += 2
    elif hematocrit < 40:
        apache_score += 1

    # White blood cell count points
    if wbc < 1 or wbc > 30:
        apache_score += 2
    elif wbc < 4 or wbc > 11:
        apache_score += 1

    # Glasgow Coma Scale points
    if glasgow_coma_scale <= 6:
        apache_score += 4
    elif glasgow_coma_scale <= 8:
        apache_score += 3
    elif glasgow_coma_scale <= 10:
        apache_score += 2
    elif glasgow_coma_scale <= 14:
        apache_score += 1

    return apache_score


# Example usage
score = calculate_apache_ii_score()
print("APACHE II Score:", score)
