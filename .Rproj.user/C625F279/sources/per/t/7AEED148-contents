source('ui.R', encoding = 'utf-8')

server <- function(input, output){
  output$mapa  <- renderLeaflet({
    mapa
  })
  
  output$plot1  <- renderPlotly({
    plotConfirmados
  })
  
  output$plot2  <- renderPlotly({
    plotObitos
  })
  
  output$plot3  <- renderPlotly({
    plotNovosCasos
  })
  
  output$plot4  <- renderPlotly({
    plotNovosCasosObito
  })
  
  output$tabset1Selected  <-  renderPlotly({
    input$tabset1
  })
  
}
