# Use Neon Managed Better Auth and Vercel Hobby

**Status:** Accepted

This is a family gift-list app expected to see intermittent, seasonal use. We will use Neon Postgres with Managed Better Auth on its free plan, and deploy the Next.js app on Vercel Hobby, which is intended for personal, non-commercial projects. Neon compute scales to zero when idle and wakes on the next database request, avoiding Supabase Free's inactivity pause while keeping initial hosting costs at zero.

The trade-offs are a brief cold start after idle periods, monthly free-tier limits that can suspend compute if exceeded, and limited backup options. Access control for shared lists and private recipients is security-critical: verify how Managed Better Auth identity is enforced for database access, and cover the authorization rules with tests before storing real family data. Supabase Pro remains an alternative if its more integrated Auth-to-RLS path is needed; it starts at $25/month and avoids inactivity pauses.