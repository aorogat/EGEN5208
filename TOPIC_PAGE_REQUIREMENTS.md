# Topic Page Requirements Specification

**Document Purpose:** This specification defines the design, content, and evaluation standards for all topic pages in the EGEN Topics course module. It serves as:
- Design guidelines for page implementation
- Presentation requirements for students
- Grading rubric for instructors

**Applicability:** All topic pages (Topic 1 through Topic 8)

---

## 1. Visual & Structural Requirements

### 1.1 Design Consistency (MANDATORY)

Topic pages must maintain visual consistency with the index page:

**Required Elements:**
- Same font family: `system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Arial, sans-serif`
- Same base font size: `14px`
- Same maximum width: `960px` (centered layout)
- Same color palette:
  - Text: `#222` (headings), `#333` (body)
  - Links: `#1a5490` (muted blue)
  - Subtle text: `#555`, `#666`
- Same spacing philosophy: dense, readable, information-first
- Same line height: `1.5`

**Explicitly Forbidden:**
- ❌ Cards, panels, or boxed sections with backgrounds
- ❌ Background colors per section
- ❌ Decorative icons or graphics
- ❌ Animations, transitions, or hover effects (except basic link underline)
- ❌ Rounded corners, shadows, or gradients
- ❌ Marketing-style callouts or promotional language

**Design Principle:** The topic page should feel like a continuation of the index page, not a new design system.

### 1.2 Page Structure (Required Sections)

Each topic page must contain the following sections in this exact order:

1. **Navigation**
   - Simple text link: `← Back to Topics` linking to `index.html`
   - No breadcrumb graphics, icons, or button styling
   - Minimal spacing above content

2. **Topic Header**
   - Topic number and full title (e.g., "Topic 1: NoSQL – Graph-Oriented Databases")
   - One-line formal subtitle (e.g., "Property Graph Model, Neo4j Architecture, and Cypher Query Language")
   - No marketing language or hype words

3. **Topic Overview**
   - Short academic paragraph (3-4 sentences) explaining:
     - Why this topic matters in modern database systems
     - Where it fits in the broader landscape
     - What students are expected to learn
   - Formal, precise language

4. **Student Presentation Assignments**
   - Clearly separated sections for Student 1, Student 2, Student 3, Student 4
   - Each section must include:
     - Clear label (e.g., "Student 1:")
     - Descriptive presentation title
     - Explicit required coverage points (bullet list)
     - Expected depth indicators

5. **Presentation Requirements**
   - Shared requirements applicable to all students
   - Time limits and structure expectations
   - Depth and scope requirements

6. **Evaluation Criteria**
   - Transparent grading breakdown
   - Rubric with weights
   - Focus on understanding, clarity, and rigor

7. **Recommended References**
   - Curated, high-quality technical sources
   - Mix of textbooks, official documentation, and academic material
   - Proper citations and links

---

## 2. Student Presentation Requirements

### 2.1 Time & Scope

**Hard Requirements:**
- Duration: 20–25 minutes per presentation
- Must cover core concepts + system-level understanding
- Must go beyond definitions and include design trade-offs

**Critical Rule:**
> Slides that only summarize definitions or list features will receive low marks. Presentations must demonstrate understanding of trade-offs, limitations, and practical considerations.

### 2.2 Required Presentation Structure (All Students)

Every presentation must include these five components:

1. **Problem Context**
   - What problem this technology or concept solves
   - Why traditional databases struggle with this problem
   - Historical context or motivation

2. **Core Concepts**
   - Clear explanation of the underlying model or mechanism
   - Correct technical terminology
   - Formal definitions where appropriate

3. **System or Language Details**
   - How it works in practice (architecture, query model, execution)
   - Concrete examples (code, diagrams, or data structures)
   - Implementation-level understanding

4. **Trade-offs**
   - Strengths and limitations
   - When it is appropriate and when it is not
   - Performance, consistency, or complexity trade-offs
   - Comparison with alternatives

5. **Real-World Perspective**
   - At least one realistic application scenario
   - Discussion of production considerations
   - Operational challenges or best practices

### 2.3 Presentation Quality Standards

**Required:**
- Clear slide structure with logical flow
- Appropriate use of diagrams, code examples, or visualizations
- Professional formatting and readability
- Time management (stay within 20–25 minutes)

**Strongly Encouraged:**
- Live demonstrations or examples
- Comparison tables or diagrams
- Real-world case studies

**Penalties:**
- Reading slides verbatim: significant penalty
- Overly simplified explanations: marks deducted
- Missing trade-offs or limitations: marks deducted

---

## 3. Topic-Specific Coverage Requirements

### Example: Topic 1 – Graph-Oriented Databases

**Student 1: Graph Data Models & Use Cases**

**Must Cover:**
- Formal definition of graph databases
- Property graph model (nodes, relationships, properties) with examples
- Comparison with relational and document models (expressiveness vs performance)
- Representative use cases (social networks, recommendation systems, fraud detection, knowledge graphs)
- Clear explanation of when graph databases are a poor choice
- Trade-offs: query complexity, scalability, consistency models

**Student 2: Neo4j Architecture & Storage**

**Must Cover:**
- High-level Neo4j architecture (components and data flow)
- Native graph storage and index-free adjacency concept
- Transaction model and ACID guarantees
- Clustering and replication design
- Scalability limits and bottlenecks
- Comparison with graph databases that use relational backends

**Student 3: Cypher Query Language**

**Must Cover:**
- Cypher's pattern-matching paradigm
- Core query constructs (MATCH, CREATE, WHERE, RETURN) with examples
- Comparison with SQL joins (conceptual and performance differences)
- Variable-length paths and graph traversals
- Performance considerations and query optimization
- Typical query anti-patterns

**Student 4: Graph Analytics & Applications**

**Must Cover:**
- Graph algorithms supported by Neo4j GDS (PageRank, shortest path, community detection)
- Analytical vs transactional workloads
- Example real-world applications (LinkedIn, recommendation engines)
- Integration with ML or recommendation systems
- Production strengths and weaknesses
- When to use graph analytics vs other approaches

**Note:** Similar detailed coverage requirements apply to all topics (2–8). Each topic page must specify topic-specific requirements for all four student assignments.

---

## 4. Evaluation Criteria (Transparent Grading)

### 4.1 Grading Rubric

Each presentation will be evaluated using the following rubric:

| Criterion | Weight | Description |
|-----------|--------|-------------|
| **Technical Correctness** | 30% | Accuracy of technical content, correct use of terminology, absence of errors |
| **Depth of Understanding** | 25% | Goes beyond surface-level definitions, demonstrates system-level comprehension |
| **Clarity and Structure** | 20% | Logical flow, clear explanations, appropriate use of examples and visuals |
| **Use of Examples and Trade-offs** | 15% | Concrete examples, discussion of limitations, comparison with alternatives |
| **Slide Quality and Time Management** | 10% | Professional formatting, appropriate pacing, stays within time limit |

### 4.2 Grading Notes

**High Marks (A range):**
- Demonstrates deep understanding beyond definitions
- Includes thoughtful trade-off analysis
- Uses concrete examples effectively
- Clear, well-structured presentation
- Stays within time limit

**Medium Marks (B range):**
- Correct but surface-level coverage
- Some examples but limited trade-off discussion
- Generally clear but could be more structured
- Minor time management issues

**Low Marks (C range or below):**
- Only definitions or feature lists
- No trade-off analysis
- Unclear or poorly structured
- Significant time management problems
- Technical errors or misunderstandings

**Penalties:**
- Reading slides verbatim: -10 points
- Overly simplified explanations: -5 to -10 points
- Missing required coverage: -5 points per missing element
- Exceeding time limit significantly: -5 points

### 4.3 Consistency

TAs and instructors should use this rubric consistently. The topic page itself should be sufficient for grading without additional documentation.

---

## 5. Reference & Source Requirements

### 5.1 Required Source Quality

**Acceptable Sources:**
- Official documentation (vendor or project)
- Academic textbooks or survey papers
- Reputable engineering blogs with clear citations
- Conference papers (SIGMOD, VLDB, etc.)
- Well-regarded technical books (O'Reilly, etc.)

**Not Acceptable as Primary Sources:**
- Medium articles without references
- AI-generated explanations (ChatGPT, etc.)
- Wikipedia as the main source
- Uncited blog posts or tutorials
- Marketing materials or vendor promotional content

**Citation Requirements:**
- All sources must be properly cited
- Students should use multiple sources (minimum 3–5)
- Mix of documentation, academic, and practical sources

### 5.2 Recommended References Format

Each topic page should include a "Recommended References" section with:

**Books:**
- Author, Title, Publisher, Year
- Brief note on relevance

**Documentation:**
- Official documentation links
- Specific sections or manuals

**Academic / Technical:**
- Survey papers or key research papers
- Conference proceedings
- Technical reports

**Example (Topic 1):**

**Books:**
- Robinson, Ian et al. *Graph Databases*. O'Reilly Media, 2015.
- Kleppmann, Martin. *Designing Data-Intensive Applications*. O'Reilly Media, 2017.

**Documentation:**
- Neo4j Official Documentation: https://neo4j.com/docs/
- Cypher Manual: https://neo4j.com/docs/cypher-manual/
- Neo4j Graph Data Science: https://neo4j.com/docs/graph-data-science/

**Academic / Technical:**
- Survey papers on graph data management (SIGMOD, VLDB proceedings)
- Neo4j Graph Data Science documentation and algorithms reference

---

## 6. Tone & Language Requirements

### 6.1 Writing Style

All text on topic pages must:

**Required:**
- Be formal and academic
- Use precise technical terms
- Avoid promotional language
- Be clear and direct

**Forbidden:**
- ❌ Emojis or casual language
- ❌ Buzzwords or hype ("revolutionary", "cutting-edge", "powerful")
- ❌ Marketing language ("leverage", "unlock", "empower")
- ❌ Exclamation points (except in rare cases)
- ❌ Casual contractions in formal sections

**Tone Examples:**

❌ **Wrong:** "Graph databases are revolutionary! They unlock powerful new ways to model data."

✅ **Correct:** "Graph databases provide a data model optimized for relationship-heavy queries. They are appropriate when the structure of connections between entities is central to the application."

### 6.2 Target Audience

The page should read like:
- A graduate course handout
- A technical specification document
- An academic syllabus section

**Not like:**
- A blog post
- A marketing page
- A tutorial or "getting started" guide

---

## 7. Success Criteria

### 7.1 Student Perspective

A topic page is successful if:
- A student understands exactly what is expected for their presentation
- A student knows what sources are acceptable
- A student can prepare without additional clarification
- The requirements are unambiguous

### 7.2 Instructor/TA Perspective

A topic page is successful if:
- A TA could grade consistently using only this page
- The evaluation criteria are clear and unambiguous
- The requirements are specific enough to prevent interpretation issues
- The page serves as a complete reference for the topic

### 7.3 Design Perspective

A topic page is successful if:
- It looks appropriate on a university website
- It maintains visual consistency with the index page
- It feels like part of a cohesive course module
- It does not draw attention to itself (content-first design)

---

## 8. Implementation Checklist

When creating or updating a topic page, verify:

- [ ] Visual consistency with index page (fonts, colors, spacing)
- [ ] All required sections present and in order
- [ ] Topic overview is formal and academic
- [ ] All four student assignments clearly defined
- [ ] Presentation requirements section included
- [ ] Evaluation criteria with weights specified
- [ ] Recommended references with proper citations
- [ ] No cards, backgrounds, or decorative elements
- [ ] No animations or transitions
- [ ] Language is formal and precise
- [ ] No marketing or promotional language
- [ ] Links are relative (GitHub Pages compatible)
- [ ] Mobile responsive (tested at 768px breakpoint)

---

## Document Version

**Version:** 1.0  
**Last Updated:** [Current Date]  
**Status:** Active Specification

**Notes:** This document should be referenced when creating or updating any topic page. It ensures consistency, clarity, and fairness across all topics in the course module.

