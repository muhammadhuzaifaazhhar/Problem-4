# Problem-4
def compute_bowling_stats(scores, handicap):
    average_score = sum(scores) / len(scores)
    average_score_with_handicap = average_score + handicap
    return average_score, average_score_with_handicap

last_name = input("Enter bowler's last name: ")
game_scores = [float(input(f"Enter game score {i+1}: ")) for i in range(3)]
handicap = float(input("Enter handicap: "))

average_score, average_score_with_handicap = compute_bowling_stats(game_scores, handicap)

print(f"Last Name: {last_name}")
print(f"Average Score: {average_score}")
print(f"Average Score with Handicap: {average_score_with_handicap}")
