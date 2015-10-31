# no-buffering-workaround
This package exists as a workaround for GHC bug #2189, "`hSetBuffering stdin
NoBuffering` doesn't work on Windows". It provides functionality for reading
from standard input without buffering, in a way that works under GHC on
Windows as well as other configurations. This is useful for key-driven console
applications such as roguelikes.
