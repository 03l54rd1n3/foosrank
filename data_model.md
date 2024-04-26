# Data Model

## player

- id: int
- first_name: string
- last_name: string
- picture_url: string

## organization

- id: string
- name: string

## player_organization

- player_id: int
- organization_id: string
- player_number: int
- profile_url: string

## singles_match

- id: int
- datetime: datetime
- player1_id: int
- player2_id: int
- player1_score: int
- player2_score: int
- result: int
- match_source_id: int

## doubles_match

- id: int
- datetime: datetime
- player1_id: int
- player2_id: int
- player3_id: int
- player4_id: int
- team1_score: int
- team2_score: int
- result: int
- match_source_id: int

## match_source

- id: int
- name: string

## elo_rating

- player_id: int
- datetime: datetime
- rating: int