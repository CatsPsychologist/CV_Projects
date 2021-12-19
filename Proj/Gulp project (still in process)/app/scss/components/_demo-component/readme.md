Component should have some structure
    
    Component Folder (name should start from '_' )
    Example: '_demo-component'

    Component Desktop styles (same as folder name but without '_' )
    Example: 'demo-component.scss'

    Component Media styles (for small screens) (same as folder name 
    but with suffix '-media' and widthot '-' too)
    Example: 'demo-component-media.scss'

    Component index file (sould be always 'index.scss')
    In your component index you sould import all you previous files:
    
    Example:
    import Component Desctop styles (@import './'demo-component.scss')
    import Component media styles (@import './'demo-component-media.scss')

    P.S If you need some extra styles 
    Example: you need to import bootstrap carousel styles to make you 
    component work with a single import - you need to import that styles
    to index file of your component
    

    Structure example:

        _demo-component (folder)
            - demo-component.scss (desktop)
            - demo-component-media.scss (media)
            - index.scss
                - @import 'bootstrap/scss/carousel'
                - @import './demo-component' 
                - @import './demo-component-media' 
        