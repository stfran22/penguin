library(glue)
library(tools)

create_scatterplot <- function(data, island, species) {
  data %>% 
    filter(species==species, island==island) %>% 
    ggplot(aes(x=bill_length_mm, y=bill_depth_mm)) +
    geom_point(size = 3) +
    labs(title = glue("{toTitleCase(species)}"), 
         x = "Bill Length (mm)", 
         y = "Bill Depth (mm)") +
    scale_x_continuous(breaks = seq(30, 60, by = 5)) +  # Adjust x-axis ticks
    scale_y_continuous(breaks = seq(10, 25, by = 2)) # Adjust y-axis ticks 
}


library(ggplot2)

theme_drexel <- function() {
  theme_minimal() +
    theme(
      text = element_text(family = "Lato", color = "#07294D"),  # Drexel Blue text
      plot.title = element_text(size = 18, face = "bold", hjust = 0.5, color = "#07294D"),
      plot.subtitle = element_text(size = 14, hjust = 0.5, color = "#07294D"),
      axis.title = element_text(size = 14, face = "bold", color = "#07294D"),  # Drexel Gold axis titles
      axis.text = element_text(size = 12, color = "#07294D"),  # Drexel Blue axis text
      panel.grid.major = element_line(color = "#D5D8DC"),  # Light gray grid
      panel.grid.minor = element_blank(),  # Hide minor grid
      plot.background = element_rect(fill = "white", color = NA),
      panel.background = element_rect(fill = "white", color = NA),
      legend.background = element_rect(fill = "white", color = NA),
      legend.position = "top",
      legend.title = element_text(face = "bold", color = "#07294D"),  # Drexel Gold legend title
      legend.text = element_text(size = 12, color = "#07294D")
    )
}

