# guardar-cap

- [ ] guardar en el ordenador el capitulo por el que vas dependiendo de la serie

hist_dir="${ANI_CLI_HIST_DIR:-${XDG_STATE_HOME:-$HOME/.local/state}/ani-cli}"
[ ! -d "$hist_dir" ] && mkdir -p "$hist_dir"
histfile="$hist_dir/ani-hsts"
[ ! -f "$histfile" ] && : >"$histfile"
search="${ANI_CLI_DEFAULT_SOURCE:-scrape}"

basicamente crear un fichero que guarde el nombre del anime y el episodio por el que vas
hay que modificar el script para que si haces -c (continuar) te salga la lista con los animes que puedes continuar
