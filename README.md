export default function TripleAmazingPlaceholder() {
  return (
    <div className="min-h-screen bg-black text-white antialiased selection:bg-white/10">
      {/* Ambient glow backdrop */}
      <div className="pointer-events-none fixed inset-0 [background:radial-gradient(900px_600px_at_50%_-10%,rgba(168,85,247,0.18),transparent),radial-gradient(700px_400px_at_110%_10%,rgba(124,58,237,0.14),transparent),radial-gradient(700px_500px_at_-10%_30%,rgba(59,130,246,0.10),transparent)]" />

      {/* Minimal header brand */}
      <header className="relative z-10 mx-auto flex w-full max-w-6xl items-center justify-between px-6 py-6">
        <div className="flex items-center gap-3 text-sm tracking-[0.22em] text-white/70">
          <span className="font-semibold">TRIPLE AMAZING</span>
          <sup className="align-super">³</sup>
        </div>
        <a
          href="mailto:hello@tripleamazing.com?subject=Stay%20in%20the%20loop"
          className="relative rounded-xl border border-white/10 bg-white/5 px-3 py-1.5 text-xs font-medium text-white/80 backdrop-blur transition hover:bg-white/10 hover:shadow-[0_0_12px_rgba(167,139,250,0.6)]"
        >
          hello@tripleamazing.com
          <span className="absolute inset-0 animate-ping rounded-xl bg-white/10 opacity-0 hover:opacity-100" />
        </a>
      </header>

      {/* Hero: make the message the main event */}
      <main className="relative z-10 mx-auto flex min-h-[70vh] max-w-6xl flex-col items-center justify-center px-6 text-center">
        {/* Soft triangle watermark behind the text */}
        <svg
          width="480"
          height="480"
          viewBox="0 0 120 120"
          className="pointer-events-none absolute -top-10 left-1/2 -z-10 -translate-x-1/2 opacity-20 blur-[1px]"
          fill="none"
        >
          <defs>
            <linearGradient id="g2" x1="0" y1="0" x2="120" y2="120" gradientUnits="userSpaceOnUse">
              <stop offset="0%" stopColor="#A855F7" />
              <stop offset="50%" stopColor="#7C3AED" />
              <stop offset="100%" stopColor="#60A5FA" />
            </linearGradient>
          </defs>
          <path d="M60 10 L110 100 H10 Z" stroke="url(#g2)" strokeWidth="1.5" />
        </svg>

        <div className="mb-5 text-xs uppercase tracking-[0.35em] text-white/50">We’re building</div>

        <h1 className="leading-[0.9] text-5xl sm:text-6xl md:text-7xl lg:text-8xl font-extrabold">
          <span className="block bg-gradient-to-br from-white via-white to-white/70 bg-clip-text text-transparent drop-shadow-[0_0_30px_rgba(167,139,250,0.35)]">
            AMAZING
          </span>
          <span className="block bg-gradient-to-r from-indigo-200 via-white to-indigo-200 bg-clip-text text-transparent opacity-90">
            AMAZING
          </span>
          <span className="block bg-gradient-to-tr from-violet-200 via-white to-blue-200 bg-clip-text text-transparent">
            AMAZING<sup className="ml-1 align-super text-base">³</sup>
          </span>
        </h1>

        <p className="mt-6 max-w-xl text-sm sm:text-base text-white/70">
          A minimal work‑in‑progress space while we craft the full experience.
        </p>

        {/* Actions */}
        <div className="mt-8 flex flex-col items-center gap-3 sm:flex-row">
          <a
            href="mailto:hello@tripleamazing.com?subject=Stay%20in%20the%20loop"
            className="rounded-2xl border border-white/15 bg-white/5 px-5 py-3 text-sm font-medium backdrop-blur transition hover:bg-white/10"
          >
            Say hi — hello@tripleamazing.com
          </a>
          <div className="text-white/40 text-sm">or</div>
          <div className="flex items-center gap-2 text-sm text-white/70">
            <a href="https://instagram.com/triple.amazing" target="_blank" rel="noreferrer" className="underline-offset-4 hover:underline">
              @triple.amazing
            </a>
            <span>•</span>
            <a href="https://instagram.com/staytripleamazing" target="_blank" rel="noreferrer" className="underline-offset-4 hover:underline">
              @staytripleamazing
            </a>
          </div>
        </div>
      </main>

      {/* Divider */}
      <div className="mx-auto mt-14 h-px w-24 max-w-6xl bg-gradient-to-r from-transparent via-white/20 to-transparent" />

      {/* Footer */}
      <footer className="mx-auto max-w-6xl px-6 py-6 text-center text-xs text-white/50">
        © {new Date().getFullYear()} TRIPLE AMAZING — ALL VIBES RESERVED
      </footer>

      {/* Corner sparkle */}
      <div className="pointer-events-none fixed bottom-8 right-8 hidden md:block">
        <div className="h-3 w-3 animate-ping rounded-full bg-white/40" />
      </div>
    </div>
  );
}
