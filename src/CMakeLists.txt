set(plasma-settings_SRCS
    main.cpp
    settingsapp.cpp
    modulesmodel.cpp
    module.cpp
)

add_executable(plasma-settings ${plasma-settings_SRCS})

target_link_libraries(plasma-settings
    Qt5::Quick
    Qt5::Gui
    Qt5::Widgets
    KF5::Package
    KF5::DBusAddons
    KF5::QuickAddons
    KF5::I18n
    KF5::Declarative
)

install( TARGETS plasma-settings ${INSTALL_TARGETS_DEFAULT_ARGS} )
