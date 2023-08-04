# Java compiler and flags
JAVAC = javac
JFLAGS = -d bin -sourcepath src

# Directory structure
SRCDIR = src
BINDIR = bin

# List of Java classes
CLASSES = MonteCarloMinimization Search TerrainArea

# Default target
all: $(BINDIR) $(CLASSES)

# Compile all Java classes
$(BINDIR):
	mkdir -p $(BINDIR)

$(CLASSES): $(BINDIR)/%.class : $(SRCDIR)/%.java
	$(JAVAC) $(JFLAGS) $<

# Clean build files
clean:
	rm -rf $(BINDIR)

# Clean and recompile
rebuild: clean all
