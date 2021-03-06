###############################################################################
#  Copyright (c) 2014-2015 libbitcoin-network developers (see COPYING).
#
#         GENERATED SOURCE CODE, DO NOT EDIT EXCEPT EXPERIMENTALLY
#
###############################################################################

# Automake settings.
#==============================================================================
# Look for macros in the m4 subdirectory.
#------------------------------------------------------------------------------
ACLOCAL_AMFLAGS = -I m4


# Distribute, make and install products.
#==============================================================================
# files => ${pkgconfigdir}
#------------------------------------------------------------------------------
pkgconfig_DATA = \
    libbitcoin-network.pc

# files => ${docdir}
#------------------------------------------------------------------------------
doc_DATA = \
    AUTHORS \
    COPYING \
    ChangeLog \
    INSTALL \
    NEWS \
    README

# src/libbitcoin-network.la => ${libdir}
#------------------------------------------------------------------------------
lib_LTLIBRARIES = src/libbitcoin-network.la
src_libbitcoin_network_la_CPPFLAGS = -I${srcdir}/include ${bitcoin_CPPFLAGS}
src_libbitcoin_network_la_LIBADD = ${bitcoin_LIBS}
src_libbitcoin_network_la_SOURCES = \
    src/acceptor.cpp \
    src/channel.cpp \
    src/connector.cpp \
    src/hosts.cpp \
    src/message_subscriber.cpp \
    src/p2p.cpp \
    src/proxy.cpp \
    src/settings.cpp \
    src/protocols/protocol.cpp \
    src/protocols/protocol_address_31402.cpp \
    src/protocols/protocol_events.cpp \
    src/protocols/protocol_ping_31402.cpp \
    src/protocols/protocol_ping_60001.cpp \
    src/protocols/protocol_reject_70002.cpp \
    src/protocols/protocol_seed_31402.cpp \
    src/protocols/protocol_timer.cpp \
    src/protocols/protocol_version_31402.cpp \
    src/protocols/protocol_version_70002.cpp \
    src/sessions/session.cpp \
    src/sessions/session_batch.cpp \
    src/sessions/session_inbound.cpp \
    src/sessions/session_manual.cpp \
    src/sessions/session_outbound.cpp \
    src/sessions/session_seed.cpp

# local: test/libbitcoin-network-test
#------------------------------------------------------------------------------
if WITH_TESTS

TESTS = libbitcoin-network-test_runner.sh

check_PROGRAMS = test/libbitcoin-network-test
test_libbitcoin_network_test_CPPFLAGS = -I${srcdir}/include ${bitcoin_CPPFLAGS}
test_libbitcoin_network_test_LDADD = src/libbitcoin-network.la ${boost_unit_test_framework_LIBS} ${bitcoin_LIBS}
test_libbitcoin_network_test_SOURCES = \
    test/main.cpp \
    test/p2p.cpp

endif WITH_TESTS

# files => ${includedir}/bitcoin
#------------------------------------------------------------------------------
include_bitcoindir = ${includedir}/bitcoin
include_bitcoin_HEADERS = \
    include/bitcoin/network.hpp

include_bitcoin_networkdir = ${includedir}/bitcoin/network
include_bitcoin_network_HEADERS = \
    include/bitcoin/network/acceptor.hpp \
    include/bitcoin/network/channel.hpp \
    include/bitcoin/network/connector.hpp \
    include/bitcoin/network/define.hpp \
    include/bitcoin/network/hosts.hpp \
    include/bitcoin/network/message_subscriber.hpp \
    include/bitcoin/network/p2p.hpp \
    include/bitcoin/network/proxy.hpp \
    include/bitcoin/network/settings.hpp \
    include/bitcoin/network/version.hpp

include_bitcoin_network_protocolsdir = ${includedir}/bitcoin/network/protocols
include_bitcoin_network_protocols_HEADERS = \
    include/bitcoin/network/protocols/protocol.hpp \
    include/bitcoin/network/protocols/protocol_address_31402.hpp \
    include/bitcoin/network/protocols/protocol_events.hpp \
    include/bitcoin/network/protocols/protocol_ping_31402.hpp \
    include/bitcoin/network/protocols/protocol_ping_60001.hpp \
    include/bitcoin/network/protocols/protocol_reject_70002.hpp \
    include/bitcoin/network/protocols/protocol_seed_31402.hpp \
    include/bitcoin/network/protocols/protocol_timer.hpp \
    include/bitcoin/network/protocols/protocol_version_31402.hpp \
    include/bitcoin/network/protocols/protocol_version_70002.hpp

include_bitcoin_network_sessionsdir = ${includedir}/bitcoin/network/sessions
include_bitcoin_network_sessions_HEADERS = \
    include/bitcoin/network/sessions/session.hpp \
    include/bitcoin/network/sessions/session_batch.hpp \
    include/bitcoin/network/sessions/session_inbound.hpp \
    include/bitcoin/network/sessions/session_manual.hpp \
    include/bitcoin/network/sessions/session_outbound.hpp \
    include/bitcoin/network/sessions/session_seed.hpp

