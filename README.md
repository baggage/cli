# baggage

Command line tool for the baggage.io web-to-email API.

# installation

The tool is just a bash script, so it's very easy to install.

    $ curl -sL -o baggage http://tool.baggage.io && chmod +x baggage

For more convenience, move it to /usr/bin/

    sudo mv baggage /usr/bin/

# usage

    $ baggage help

    Usage: baggage COMMAND [OPTS]

    Commands:

        subscribe EMAIL [OPTS]

            Subscribes email address. Options are:

            -n --name       Descriptive name
            -e --expires    Inactivity expiry time

        stats

            Retrieves stats for subscription.

        update [OPTS]

            Updates subscription. Options are:

            -n --name       Descriptive name
            -e --expires    Inactivity expiry time

        rotate

            Rotates tokens.

        unsubscribe

            Unsubscribes.

        send SUBJECT [OPTS] [BODY]

            Sends email. Options are:

            -f --from       Email from name

            If BODY is not provided, it is read from STDIN.

        ping

            Basic connectivity test.

        version

            Prints version

        help

            This help.

            See https://github.com/baggage/app for full API docs


# contributing

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request


