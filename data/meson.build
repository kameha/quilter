icon_sizes = ['16', '24', '32', '48', '64', '128']

foreach i : icon_sizes
    install_data(
        join_paths('icons', i, meson.project_name() + '.svg'),
        install_dir: join_paths(get_option('datadir'), 'icons', 'hicolor', i + 'x' + i, 'apps')
    )
endforeach

foreach i : icon_sizes
    install_data(
        join_paths('icons', i, meson.project_name() + '.svg'),
        install_dir: join_paths(get_option('datadir'), 'icons', 'hicolor', i + 'x' + i + '@2', 'apps')
    )
endforeach

install_data(
    meson.project_name() + '.gschema.xml',
    install_dir: join_paths(get_option('datadir'), 'glib-2.0', 'schemas')
)

install_data(
    meson.project_name() + '.desktop',
    install_dir: join_paths(get_option('datadir'), 'applications')
)

install_data(
    meson.project_name() + '.appdata.xml',
    install_dir: join_paths(get_option('datadir'), 'metainfo')
)

install_data(
    join_paths('schemes', 'quilter.xml'),
    install_dir: join_paths(get_option('datadir'), 'gtksourceview-3.0', 'styles')
)

install_data(
    join_paths('schemes', 'quilter-dark.xml'),
    install_dir: join_paths(get_option('datadir'), 'gtksourceview-3.0', 'styles')
)

install_data(
    join_paths('font', 'PTM55FT.ttf'),
    install_dir: join_paths(get_option('datadir'), 'fonts', 'truetype', 'pt-mono')
)

install_subdir(
    'highlight.js',
    install_dir: join_paths([ get_option('prefix'), get_option('datadir'), 'com.github.lainsce.quilter' ])
)
