
rp_test(
  UNIT_TEST
  BINARY_NAME test_http_client
  SOURCES http_client_test.cc framing_test.cc
  DEFINITIONS BOOST_TEST_DYN_LINK
  LIBRARIES v::seastar_testing_main v::application Boost::unit_test_framework v::http
  ARGS "-- -c 1"
)
