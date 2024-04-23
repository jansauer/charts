def update_catalog_file(location: str) -> None:
catalog_file_path = os.path.join(location, CACHED_CATALOG_FILE_NAME)
catalog_data, versions_data = get_trains(location)
validate_train_data(catalog_data)
validate_versions_data(versions_data)
