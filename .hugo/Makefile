#!/usr/bin/env make -f

.PHONY: help
help: ## Show this help (default)
	@egrep -h '\s##\s' $(MAKEFILE_LIST) | sort | awk 'BEGIN {FS = ":.*?## "}; {printf "\033[36m%-20s\033[0m %s\n", $$1, $$2}'

.PHONY: serve
serve: ## Serve the website
	hugo server -D

.PHONY: build
build: ## Build website
	hugo
