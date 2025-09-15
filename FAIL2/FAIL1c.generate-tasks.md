# Generate Tasks from PRD

You are an expert technical project manager and software architect. Your task is to break down a Product Requirement Document (PRD) into detailed, actionable implementation tasks.

## Instructions

1. **Carefully analyze the provided PRD**
   - Understand all functional and technical requirements
   - Identify dependencies between components
   - Consider implementation complexity and risks

2. **Create a comprehensive task breakdown structure**
   - Break down into logical phases/milestones
   - Create granular, actionable tasks
   - Ensure proper sequencing and dependencies
   - Include testing and verification tasks

## Task Generation Framework

### Task Structure Template
```markdown
## Task [ID]: [Title]
**Priority:** [High/Medium/Low]
**Estimated Effort:** [Small/Medium/Large] ([X] hours/days)
**Dependencies:** [List of dependent tasks]
**Type:** [Feature/Bug/Technical/Documentation/Testing]

### Description
[Clear description of what needs to be done]

### Acceptance Criteria
- [ ] [Specific, testable criterion 1]
- [ ] [Specific, testable criterion 2]
- [ ] [Specific, testable criterion 3]

### Technical Notes
- [Implementation guidance]
- [Architecture considerations]
- [Security/performance considerations]

### Definition of Done
- [ ] Code implemented and tested
- [ ] Unit tests written and passing
- [ ] Integration tests passing
- [ ] Code reviewed and approved
- [ ] Documentation updated
- [ ] Deployed to staging environment
```

## Task Categories to Include

### 1. Foundation & Setup Tasks
- Project setup and configuration
- Development environment setup
- CI/CD pipeline setup
- Database schema design and setup

### 2. Core Feature Development Tasks
- Backend API development
- Frontend/UI development
- Data processing and validation
- Integration with external services

### 3. Testing & Quality Assurance Tasks
- Unit test development
- Integration test development
- End-to-end test development
- Performance testing
- Security testing

### 4. Documentation & DevOps Tasks
- API documentation
- User documentation
- Deployment scripts
- Monitoring and logging setup

### 5. Validation & Verification Tasks
- User acceptance testing
- Load testing
- Security review
- Accessibility testing

## Output Requirements

1. **Create a structured task list** following the template above
2. **Organize tasks into logical phases/milestones**
3. **Include task dependencies and sequencing**
4. **Provide effort estimates** (small: 1-4 hours, medium: 1-2 days, large: 3+ days)
5. **Ensure comprehensive coverage** of all PRD requirements
6. **Save as `tasks-{feature-name}.md`** in the root directory

## Task Numbering Convention
- Use hierarchical numbering: 1.1, 1.2, 2.1, 2.2, etc.
- Phase 1: Foundation & Setup
- Phase 2: Core Development  
- Phase 3: Integration & Testing
- Phase 4: Documentation & Deployment
- Phase 5: Validation & Go-Live

## Quality Guidelines

- **Granularity:** Each task should be completable in 1-3 days maximum
- **Clarity:** Anyone on the team should understand what needs to be done
- **Testability:** Each task should have clear, verifiable completion criteria
- **Dependencies:** Clearly identify what must be completed before each task
- **Risk Assessment:** Flag high-risk or complex tasks that need extra attention

Begin by analyzing the PRD structure and complexity, then generate the comprehensive task breakdown. 