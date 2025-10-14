# Entendendo Cada Coluna

- 🆔 `recommendationid`: é identificador único para cada avaliação.  
- 👤 `author`: Um objeto contendo informações sobre o autor da avaliação. Dentro dele, você encontrará informações como: 
    - `steamid` do usuário  
    - Número de jogos que ele possui (`num_games_owned`)  
    - Número de avaliações que já fez (`num_reviews`)  
    - Tempo total jogado em minutos (`playtime_forever`)
    - Tempo jogado antes de avaliar (`playtime_at_review`)
- 🌐 `language`: O idioma em que a avaliação foi escrita (ex: `"brazilian"`, `"english"`).  
- 💬 `review`: comentário da avaliação.  
- ⏰ `timestamp_created`: A data e hora em que a avaliação foi criada, em formato **Unix Timestamp** (número de segundos desde 01/01/1970).  
- 🔁 `timestamp_updated`: A data e hora da **última atualização** da avaliação.  
- 👍 `voted_up`: Um valor **booleano (True/False)**.  
    **Significado:**  
    - `True` → O usuário recomendou o jogo.  
    - `False` → O usuário **não** recomendou o jogo.  
- 🗳️ `votes_up`: O número de outros usuários que acharam a avaliação **útil**.  
- 😂 `votes_funny`: O número de outros usuários que acharam a avaliação **engraçada**.
- ⚖️ `weighted_vote_score`: Um **placar ponderado** que a Steam usa para ordenar as avaliações, combinando votos e outros fatores.  
- 💬 `comment_count`: O número de comentários que outras pessoas fizeram na avaliação.
- 💸 `steam_purchase`: `True` se o jogo foi comprado diretamente na Steam.  
-  🎁 `received_for_free`: `True` se o autor declarou ter recebido o jogo de graça.
-  🧪 `written_during_early_access`: `True` se a avaliação foi feita durante o **acesso antecipado** do jogo.  
- 🎮 `primarily_steam_deck`: `True` se a avaliação é específica para a **experiência no Steam Deck**.
