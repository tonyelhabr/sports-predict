
# pkgs <- c("datasets", "utils", "grDevices", "graphics", "stats", "bindcpp")
# pacman::p_load(pkgs)
library("base")
library("methods")
library("datasets")
library("utils")
library("grDevices")
library("graphics")
library("stats")

suppressPackageStartupMessages(library("tidyverse"))
suppressPackageStartupMessages(library("rlang"))

paths_funcs <-
  list.files(
    path = "R",
    pattern = "func",
    recursive = FALSE,
    full.names = TRUE
  )
invisible(sapply(paths_funcs, source))
rm("paths_funcs")

config <- config::get()


invisible(utils::capture.output(import_nfl_tm()))
invisible(utils::capture.output(import_nfl_game_result()))