Новая сессия tmux new -s name_of_session
Подключение к существующей сессии после возвращения в терминал
`tmux ls` to get the session number или имя. And then
`tmux attach-session -t <session_number или имя>`